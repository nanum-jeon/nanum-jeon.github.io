    #####################################################################################################
    #### REPLICATIONS FOR: "An Introduction to G-Methods" by NANUM JEON #################################
    #### ORIGINAL AUTHORS: ASHLEY I NAIMI (ashley.naimi@pitt.edu), EDWARD H KENNEDY, STEPHEN R COLE    ##
    #### PURPOSE: Illustrate all three g-methods. #######################################################
    #####################################################################################################

    # Replication

    # Data in Table 1 
    # A0: Treatment at time 0 (for HIV)
    # A1: HIV viral load prior to time 1 (Higher -> More HIV)
    # A1: Treatment at time 1
    # Y: Mean of CD4 count (cells/mm)
    # N: Number of subjects 


    a0 <- c(0, 0, 0, 0, 1, 1, 1, 1)
    z1 <- c(0, 0, 1, 1, 0, 0, 1, 1)
    a1 <- c(0, 1, 0, 1, 0, 1, 0, 1)
    y <- c(87.288, 112.107, 119.654, 144.842, 105.282, 130.184, 137.720, 162.832)
    n <- c(209271, 93779, 60657, 136293, 134781, 60789, 93903, 210527)

    data <- data.frame(a0, z1, a1, y, n)

    # Section 1
    # Standard linear regression models in Table 2 
    # Not considering standard error estimation 

    # Crude model 
    lm(y ~ a0 + a1 + a0*a1, data = data, weights = n)

    ## 
    ## Call:
    ## lm(formula = y ~ a0 + a1 + a0 * a1, data = data, weights = n)
    ## 
    ## Coefficients:
    ## (Intercept)           a0           a1        a0:a1  
    ##     94.5611      24.0407      36.9378      -0.0225

    # Z-Adjusted model 
    lm(y ~ a0 + a1 + a0*a1 + z1, data = data, weights = n)

    ## 
    ## Call:
    ## lm(formula = y ~ a0 + a1 + a0 * a1 + z1, data = data, weights = n)
    ## 
    ## Coefficients:
    ## (Intercept)           a0           a1           z1        a0:a1  
    ##    87.24660     17.98931     24.96985     32.55024      0.05409

    # A0 only model 
    lm(y ~ a0, data = data, weights = n)

    ## 
    ## Call:
    ## lm(formula = y ~ a0, data = data, weights = n)
    ## 
    ## Coefficients:
    ## (Intercept)           a0  
    ##      111.56        27.08

    # Z1-Adjusted A0 Only Model
    lm(y ~ a0 + z1, data = data, weights = n)

    ## 
    ## Call:
    ## lm(formula = y ~ a0 + z1, data = data, weights = n)
    ## 
    ## Coefficients:
    ## (Intercept)           a0           z1  
    ##       94.98        18.03        42.09

    # A1 Only Model
    lm(y ~ a1, data = data, weights = n)

    ## 
    ## Call:
    ## lm(formula = y ~ a1, data = data, weights = n)
    ## 
    ## Coefficients:
    ## (Intercept)           a1  
    ##      105.59        38.91

    # Z1-Adjusted A1 Only Model
    lm(y ~ a1 + z1, data = data, weights = n)

    ## 
    ## Call:
    ## lm(formula = y ~ a1 + z1, data = data, weights = n)
    ## 
    ## Coefficients:
    ## (Intercept)           a1           z1  
    ##       94.30        25.01        36.42

    # G-formula 
