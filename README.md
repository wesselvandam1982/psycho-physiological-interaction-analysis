# psycho-physiological-interaction-analysis

# This is a pre-processing script that does the exact same steps as the original preprocessing
# script for the Emotion Regulation study, with the only difference that we use a slightly different
# function to model the HRF (i.e., BLOCK instead of the WAVE form). This is just to keep it compatible
# with the next scripts that we will use for building the PPI regressors.

# You can use 'BLOCK' for event-related analyses just by setting the duration to a small value, e.g.,
# 'BLOCK(1,1)'

# There is a number of files that are generated during this preprocessing step that we will need in further steps
# of our analysis to build our eventual PPI model. One of the files will be the errts file that we will need in order
# to extract the PPI.seed.1D file. The errts-file is a residual (or detrended) dataset, from we which we will extract
# the time course information for our ROI of the PPI analysis. 

# Secondly we will need the hrf file X.BLOCK.1D in order to be able to build the impulse response function (IRF) for the deconvolution
# and recovolution steps.
