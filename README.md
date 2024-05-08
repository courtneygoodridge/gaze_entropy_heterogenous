# Gaze Entropy Metrics for Mental Workload Estimation are Heterogenous During Hands-Off Level 2 Automation

## Reference

**If you using any elements of this repository, please cite**: Goodridge, C. M., Goncalves, R. C., Arabian, A., Horrobin, A., Solernou, A., Lee, Y. T., ... & Merat, N. (2024). Gaze entropy metrics for mental workload estimation are heterogenous during hands-off level 2 automation. Accident Analysis & Prevention, 202, 107560.

## Overview: experimental design

This expeirment aimed to understand whether gaze entropy metrics could be used to estimate mental workload during Level 2 hands-off automation. Using the University of Leeds driving simulator, participants drove a Level 2 automated vehicle with their feet and hands away from operational controls. Participants took part in two drives, with each drive containing 10 events. Each event was comprised of 2 minute of automated driving, followed by a takeover request (TOR). Upon the TOR, the driver would have to takeover control of the vehicle and drive manually. 4 events were critical and 6 were non-critical. During one drive, participants completed an auditory 2-back during automated driving; during the other drive they did not. The data analysed in this manuscript focuses on eye movements during the automated period, with and without the auditory 2-back task.  

![image](https://github.com/courtneygoodridge/gaze_entropy_heterogenous/assets/44811378/81f88195-4c04-42b0-acb9-0f61d6335bc3)

Bayesian distributional models were fitted to understand how the mean and variance of gaze entropy metrics changed as a function of mental workload demands and the presence of lead vehicles during automated driving. A focus was placed on understanding the variance of the effects, considering that human drivers are extremely variable in their behaviours. 

## Code and analysis

### Statisical modelling 

The data needed to replicate the analysis can be found with the data folder of this repository. The csvs have self-explanatory names and relate to the NASA-TLX scores, the entropy values for each trial and participant during the 2 minutes of automated driving, 2-back performance, and participant demographic information. The model fitting and plotting is all done in the `manuscript_modelling_and_plot.Rmd` file. To run this script, clone the `gaze_entropy_heterogenous` repository into your working directory (you can find this by running the `here::here()` function in the R command line). For more information on using the `here::here()`, see the [documentation](https://here.r-lib.org/). Once the repository is in your working directory, run each chunk of code to run the models and analysis. The fitting of the models is computationally heavy, and thus the model fits have been saved and are contained within the models folder. They can be re-loaded using the same script (rather than re-fitting the models). 

Raw data for pre-processing is not available due to IP restrictions. If more information is needed regarding this, please contact me (c.m.goodridge@leed.ac.uk). 
