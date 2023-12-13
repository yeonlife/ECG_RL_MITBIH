# Anomaly detection on ECG with Reinforcement Learning

The primary objective of this project is to investigate the application of Reinforcement Learning techniques 
in enhancing anomaly detection within ECG systems. By leveraging RL, we aim to develop a model 
that can adapt to automatic alerting system in mobile devices, learn from historical data, and 
identify anomalies in real-time, thereby improving the overall safety and performance of ECG data.

## Installation and Usage

This project is designed to be executed on Google Colab and involves the following components:

- 'ECG_RL.ipynb': main file for this project
- 'mithib.zip': MIT-BIH dataset

1. Upload the 'ECG_RL.ipynb' notebook to Google Colab.
2. Upload and unzip the 'mithib.zip data file in Colab. Make sure to modify the data file path in the notebook accordingly. 
'''\python
! unzip /content/drive/MyDrive/RL_project/mitbih.zip
'''
3. Open the notebook and execute the cells. To examine data for a specific patient, modify the file name in the following cell:

'''\python
patient_100_file = "/content/103.csv"
ecg100 = pd.read_csv(patient_100_file, index_col=0)
ecg100
'''

## Methodology

- [x] Wavelet Tranformation
- [x] Savitzky-Golay Filter
- [x] Q-Table Learning


## Experiment Results

[[patient 100](images/patient%20100%20threshold%202.5%20graph.png)]
[[patient 101](images/patient%20101%20threshold%202.5%20graph.png)]
[[patient 114](images/patient%20114%20threshold%202.5%20graph.png)]
[[patient 115](images/patient%20115%20threshold%202.5%20graph.png)]
[[patient 103](images/patient%20103%20threshold%202.5%20graph.png)]