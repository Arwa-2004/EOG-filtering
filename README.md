# EOG-filtering

In this project I used EOG (Electrooculography) data obtained from a subject through BIOPAC after connecting channel 1&2 electrodes to their right places as shown in the picture. The subject was required to move they eye in horizontal and vertical motion, and was required to do tasks such as reading. Then by using python (scipy) I applied bandpass, notch filter, and ICA to remove motion artifacts.

<p align="center">
<img width="213" height="498" alt="image" src="https://github.com/user-attachments/assets/a88fd9cc-0919-40ee-b89d-0838bf8a728c" />

## Data 📂 

The project expects BIOPAC ACQ files (example: GRPOUP-11-L10-L10.acq).
Make sure the file is in the working directory before running.

## Workflow📊

1. Loaded data from BIOPAC ACQ file

2. Explored channels (horizontal eye movement & vertical EOG)

3. Applied bandpass filter (0.1–30 Hz)

4. Applied notch filter (50 Hz, Q=30)

5. Applied ICA to remove eye/motion artifacts

6. Visualized results

## Results

EOG signal before filtering the horizontal channel  

<img width="532" height="281" alt="image" src="https://github.com/user-attachments/assets/dc4f5c10-a512-436a-ad54-0b9240c89c2a" />

After adding the filters on both channels

<img width="924" height="514" alt="image" src="https://github.com/user-attachments/assets/c0d1d56b-1ec2-4cd0-90ba-84258e6cb6d9" />



