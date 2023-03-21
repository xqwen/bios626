# Human Activity Recognition using Wearable Sensor Technology 





## Experiment design and data collection

A group of volunteers, aged between 19 and 48, are recruited to participate in the experiment. They performed a protocol consisting of six activities: three static postures (standing, sitting, lying) and three dynamic activities (walking, walking downstairs, and walking upstairs). The experiment also recorded postural transitions that occurred between the static postures. These are: stand-to-sit, sit-to-stand, sit-to-lie, lie-to-sit, stand-to-lie, and lie-to-stand. All participants wore a smart device on the waist during the experiment. It captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz using the embedded accelerometer and gyroscope of the device. In this context, the activities are considered outcomes, and the signals measured by the smart device are considered features. 


## Data pre-processing and description

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low-frequency components. Therefore a filter with a 0.3 Hz cutoff frequency was used. From each window, a vector of 561 features was obtained by calculating variables from the time and frequency domain. The details of the 561 features are described in files ``data/data_dictionary.txt`` and ``data/feature_info.txt``.



## Data files 

Two tab-delimited text files ``data/training_data.txt`` and ``data/test_data.txt`` are provided. The training data (labeled activity information included) should be used to construct and test your ML algorithms. Apply your algorithm to the test data (containing only feature information) and predict the activity corresponding to each time window.




## Learning tasks

1. Build a binary classifier to classify the activity of each time window into static (0) and dynamic (1).
2. Build a refined multi-class classifier to classify walking (1), walking_upstairs (2), walking_downstairs (3), sitting (4), standing (5), lying (6), and static postural transition (7)



## Submission to Leaderboard

1. create a submission ID (SID) that you can identify yourself from the leaderboard. The ID should not include space or special characters, just alphbet letters and numbers. For example, you can use the last 4-digit of your umid.
2. create two text files for the two learning tasks. The binary classification result should be named "binary\_SID.txt", and the multiclass classification result should be name "multiclass\_SID.txt". Any format other than text format will *NOT* be accepted.
3. format the correpsonding classification results into a single column. In total, there should 3,162 rows in each submitted file. Importantly, do not inlcude any header and the order of the classification results should be *exactly the same* as the order of the subject features shown in the ``test_data```. 
4. carefully check the names and the format of your two submission files. Submit through the Canvas. 

You can submit as many times as you like. The leaderboard will show the evaluation of your most recent results by the release time, i.e., your new submission will overwrite your old results. The release of the Leaderboard is scheduled on every Tuesday and Friday until April 14,2023.


