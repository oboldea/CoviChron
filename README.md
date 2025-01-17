This is the main code for the paper
*************************************************************************************************
Model-informed post-pandemic COVID-19 vaccination strategies by
age and medical risk due to chronic diseases
by Otilia Boldea, Ilse Westerhof, Eric Vos, Susan van den Hof, Jantien Backer and Ganna Rozhnova
*************************************************************************************************
For questions related to the code, please email o.boldea@tilburgunivesity.edu
*************************************************************************************************

CODE:

****************************************************
Fit data
**************************************************** 
- inference.m                -> saves posteriors for parameters and state variables into Output folder, run it before you run the other files

****************************************************
Plot output from model fit
**************************************************** 
- plot_para_posteriors.m     -> plots parameter posteriors at the end of the sample
- plot_data_fit.m            -> plots fit to data
- plot_burden                -> plots posterior estimates of cumulative infections/population and hospitalizations/infection by age and risk

****************************************************
Vaccination scenarios for the future
**************************************************** 
-scenarios_uniform.m       -> generates table and plot for burden for uniform vaccination coverage across age/risk
-scenarios_risk.m          -> generates table and plot for burden for differential vaccination coverage by risk
-scenarios_age.m           -> generates table and plot for burden for differential vaccination coverage by age
-scenarios_age_risk.m      -> generates table and plot for burden for differential vaccination coverage by age/risk
 
****************************************************
FOLDERS
**************************************************** 
Data                       -> contains data for hospitalizations (by age and age/risk), seroprevalence (by age and age/risk in 6 survey rounds), 
                              population (by age/risk), contacts (by age/risk), vaccination (by age/risk), and posterior confidence intervals 
                              from Rozhnova et al (2021), https://doi.org/10.1038/s41467-021-21899-6  
Output                     -> output generated by running inference.m
Functions                  -> functions used in codes above                  
