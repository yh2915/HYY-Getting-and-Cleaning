This dataset was processed based on another raw dataset. Experiment set up and other detailed information of the orginal dataset can be found in Appendix 1 and Appendix 2 below.
This dataset was prepared by HYY on 01 Jun 2018.

********************************
**【Files within this dataset】 **
********************************
1. README.txt
2. CodeBook.txt - Indicate all the variables and summaries calculated, along with units, and any other relevant information.
3. Assignmentoutput.txt - This is the cleaned dataset which contains the summarize information for the original dataset
4. run_analysis.R - This is the R source code containing scripts which process the original dataset to the cleaned dataset output(3.Assignmentoutput.txt) 

*****************************
**【Steps of summarization】 **
*****************************
i. The test data and the train data were combined
ii. Only  the measurements on the mean and standard deviation for each measurement were extracted.
iii. Descriptive activity names were used to name the activities in the data set as following:
    1 WALKING

    2 WALKING_UPSTAIRS

    3 WALKING_DOWNSTAIRS

    4 SITTING

    5 STANDING

    6 LAYING

iv. The dataset was labeled with the variables names provided in the original dataset
v. Independent tidy data set with the average of each variable for each activity and each subject were produced and saved as "Assignmentoutput.txt"

*********************************************
**【Appendix 1: Original Experiment set up】 **
*********************************************
-Sample: Volunteers
-Sample size: 30
-Age range: 19-48
-Activities: 
    1 WALKING

    2 WALKING_UPSTAIRS

    3 WALKING_DOWNSTAIRS

    4 SITTING

    5 STANDING

    6 LAYING

-Data source: Sensor signals from a smartphone (Samsung Galaxy S II), which is wore by the volunteers while performing activities.
  i.3-axial linear acceleration(Denoted X/Y/Z) measured by embedded accelerometer at a constant rate of 50Hz
  ii. 3-axial angular velocity(Denoted X/Y/Z) measured by embedded gyroscope at a constant rate of 50Hz
-Labeling of activities:The experiments have been video-recorded to label the data manually.
-Organization of data:The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 
-Processing of data:
The sensor signals (accelerometer and gyroscope) were pre-processed by
  i.applying noise filters
  ii.sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window)
  iii.The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity.
  iiia.The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used.
  iv. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'Codebook.txt' for more details. 

*************************************************
**【Appendix 2: Information of Original dataset】**
*************************************************
Name: Human Activity Recognition Using Smartphones Dataset
Version: 1.0
Source and company information:
Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
Smartlab - Non Linear Complex Systems Laboratory
DITEN - Università degli Studi di Genova.
Via Opera Pia 11A, I-16145, Genoa, Italy.
activityrecognition@smartlab.ws
www.smartlab.ws
For each record it is provided:
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.
The dataset includes the following files:
- 'README.txt'
- 'features_info.txt': Shows information about the variables used on the feature vector.
- 'features.txt': List of all features.
- 'activity_labels.txt': Links the class labels with their activity name.
- 'train/X_train.txt': Training set.
- 'train/y_train.txt': Training labels.
- 'test/X_test.txt': Test set.
- 'test/y_test.txt': Test labels.
The following files are available for the train and test data. Their descriptions are equivalent. 
- 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30. 
- 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis. 
- 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration. 
- 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second. 
Notes: 
- Features are normalized and bounded within [-1,1].
- Each feature vector is a row on the text file.
For more information about this dataset contact: activityrecognition@smartlab.ws
License:
========
Use of this dataset in publications must be acknowledged by referencing the following publication [1] 
[1] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012
This dataset is distributed AS-IS and no responsibility implied or explicit can be addressed to the authors or their institutions for its use or misuse. Any commercial use is prohibited.
Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, Davide Anguita. November 2012.
