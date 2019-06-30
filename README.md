# LANL EarthQuake Prediction

Current scientific studies related to earthquake forecasting focus on when, where, and how large it will be. We will be using seismic signals to predict the timing of laboratory
earthquakes. The acoustic_data input signal is used to predict the time remaining before the next laboratory earthquake time_to_failure. Using seismic signals, we are to
predict the time of laboratory earthquakes.

# DATA 
We got the data from the Kaggle website( **Needed kaggle Account to download** Link: https://www.kaggle.com/c/LANL-Earthquake-Prediction/data). It consists of three different data files, which are Train.csv, test file and sample_submission.csv
The train.csv is a single, continuous training segment of experimental data. The test data is a collection of many small segments of acoustic data signals. The
sample_submission.csv file has is needed to find the failure for each segment of test data.

###### acoustic_data - the seismic signal [int16]
###### time_to_failure - the time (in seconds) until the next laboratory earthquake [float64].

# Acoustic Data 
Acoustics is the branch of physics that deals with the study of all mechanical waves in gases, liquids, and solids including topics such as vibration, sound, ultrasound and
infrasound. A scientist who works in the field of acoustics is an acoustician while someone working in the field of acoustics technology may be called an acoustical
engineer. The application of acoustics is present in almost all aspects of modern society with the most obvious being the audio and noise control industries. An acoustician is an
expert in the science of sound. Acoustics is defined by ANSI/ASA S1.1-2013 as "(a) Science of sound, including its production, transmission, and effects, including
biological and psychological effects. (b) Those qualities of a room that, together, determine its character with respect to auditory effects." The study of acoustics revolves around the
generation, propagation and reception of mechanical waves and vibrations.

# Time to failure

Time to failures is the predicted elapsed time between inherent failures of a mechanical or electronic system, during normal system operation. Time to failures can be
calculated as the arithmetic mean (average) time between failures of a system[12]. The term is used for repairable systems, while mean time to failure denotes the expected
time to failure for a non-repairable system. The definition of Time to failures depends on the definition of what is considered a failure. For complex, repairable systems,
failures are considered to be those out of design conditions which place the system out of service and into a state for repair. Failures which occur that can be left or maintained in
an unrepaired condition, and do not place the system out of service, are not considered failures under this definition. In addition, units that are taken down for routine scheduled
maintenance or inventory control are not considered within the definition of failure. The higher the Time to failures, the longer a system is likely to work before failing.

### Instructions

Download .rmd file, run it using RStudio.

#### Prerequisites

In this project, we are using RStudio(Link to download RStudio : https://www.rstudio.com/products/rstudio/download/) and R.Download required packages for using libraries 

### Solution
I have used random forest method and for evaluating model used Leave-one-out cross validation strategy. For step-by-step explaination check MLFinalProject-RandomForest.html file in this repository. And for measuring model's accuracy used Mean absolute error metric.
