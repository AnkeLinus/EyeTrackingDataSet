# EyeTrackingDataSet
This repository contains an eye tracking dataset that was used to evaluate deviations caused by vibration of a head worn eye tracking device. 

## Information about the task
All eye tracking data was recorded with a Tobii Pro Glasses 2. Ten participants attended the study. 13 targets (markers) were given in to focus for 3 seconds. The distribution is shown in [1,2]. The participants had to focus a reference marker to start the measurement. Then the participants were asked to focus on the first marker for three seconds and returning with the gaze to the reference marker for one second. This sequence were used for all 13 markers.
The measurements were repeated eight times. In each odd measurement the vibration was inactive, in each even measurement the vibration was active. Vibrations could be seen in the video. Due to data privacy the video content can't be shared. The end of each measurement can be found in the data by searching for Event(column 14): "RecordingPause". The order of focussing the markers were randomized and are given in file "Marker_sequence.xlsx". Further information on the process can be read in detail in [1].

For easier reference all markers were given a number as seen below.
![Marker distribution and references](https://github.com/AnkeLinus/EyeTrackingDataSet/issues/1#issue-1367541683)

## Information about empirical data
In the File "Empirical Data" further data regarding the participants are given. Furhter, data on the evaluation of the eye tracking device, vibrotactile feedback, and auditory feedback resulting from the vibration are presented.  

## Notes to anomalies in data
If you want to use this dataset for further evaluation, please be aware of following problems in data recording. It is suggested to exclude the given trials.
Due to an error in the Recording the data of participant 2 measurement 3 are not showing the recording of the markers. Since the goal was to test the performance of the glasses also in the periphery, outliers can be found as well as missing data since the pupil couldn't be detected in some positions. Regarding this, following markers couldn't be detected or had less than 50 values recorded:
* Participant 3 - Measurement 2 - Marker 8 and 9
* Participant 5 - Measurement 2 - Marker 4
* Participant 5 - Measurement 5 - Marker 4 and 13
* Participant 7 - Measurement 2 - Marker 4 and 13
* Participant 7 - Measurement 7 - Marker 4
* Participant 10 - Measurement 1 - Marker 4
* Participant 10 - Measurement 2 - Marker 6, 8 and 13
* Participant 10 - Measurement 3 - Marker 5

A total of 26 missing markers occur from a population of 1040 markers. The total number of markers can be calculated by 10 participants x 8 measurements x 13 markers.

In participant 9 case the recording had to be stopped after measurement 6. Therefore, data of measurement one to six is contained in the file "Data_Participant_9a.xlsx" and measurement seven and eight in "Data_Participant_9b.xlsx".  

## Further Literature
[1] A. Fischer, T. Wendt, P. Gawron, L. Stiglmeier and K. van Laerhoven. "Evaluation of Precision, Accuracy and Threshold for the Design of Vibrotactile Feedback in Eye Tracking Applications" Sensors and Measuring Systems; 21th ITG/GMA-Symposium, 2022, pp. 1-6 on IEEE.

[2] Thibeault M, Jesteen M, Beitman A. "Improved Accuracy Test Method for Mobile Eye Tracking in Usability Scenarios". Proceedings of the Human Factors and Ergonomics Society Annual Meeting. 2019;63(1):2226-2230. doi:10.1177/1071181319631083 
