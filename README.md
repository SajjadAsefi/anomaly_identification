# Anomaly Detection and Classification in Power System State Estimation

This is a code repository for the paper "**Anomaly detection and classification in power system state estimation: Combining model-based and data-driven methods**": https://www.sciencedirect.com/science/article/pii/S2352467723001248

For additional information about the workflow of the method you can take a look at the paper "**Anomaly Detection, Classification and Identification Tool (ADCIT)**" : https://www.sciencedirect.com/science/article/pii/S2665963823000027

Codes are developed in two different environment: Matlab and python.

In order to be able to run the Matlab code you must have matpower installed
The power flow has been done using OPF via matpower (version 7.0).

The column labeled as "bus" is the target column. If there are multiple buses, they are named with different numbers (e.g. 15 indicates the combination of bus 2 and 3).

The rest are feature columns and are named as:

SCADA, U: observed (i.e. SCADA) voltage magnitudes\\
SCADA, P or Q: observed (i.e. SCADA) power injection (active P or reactive Q)
FM: Forecasted measurement
EM: Estimated measurements
ES: Estimated state
ph: Phase angle
NI: Normalized innovations
EKF: Extended Kalman filter
