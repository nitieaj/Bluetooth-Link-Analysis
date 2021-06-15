# Bluetooth-Link-Analysis

## What and Why
Performance analysis of the bluetooth link of a Cardiac Heart Rate Monitoring system. This mobile user and room monitoring station have been receiving intermittent R-R display of the values on the screen.The received measured values paint an inaccurate status of the patient`s condition. The system designed for 99% availability has failed to meet specifications and serve the user. This project evaluates the design specifications, current operating conditions and makes recommendations.

## How 
Analysis of a failing Clinical Decision Support Wireless link considering the human factors that consistently influence link performance in the clinical setting.
The Customer`s Medical Heart Rate Monitoring System comprises of the following components. 
- A heart rate variability monitor strapped to the  patient`s chest. 
- Acute Patients are immobilized in the ICU.
- A wireless receiver subsystem is installed in the  monitoring room 30ft away from the bedside. 
- The equipment vendor supplied  the equipment 5years ago, tested and verified that the transmitted R-R  intervals would display on the monitoring station. 
- A mobile App enhanced to provide mobile monitoring  capabilities.

## Input
The simulated link is built to allow collection of open source Bluetooth link logs. 
Tx Controller: A  Dell Inspiron 7559 Bluetooth  interface card.
A decommissioned  phone with an activated  host controller interface(ADB) feature set [The Android Debug Bridge (ADB) tool is part of the Android Open Source  Project.(AOSP) Specification Page] ( https://source.android.com/setup/build/adb ) 
Wireshark  network Protocol Analyzer cross sectional data 

## Algorithm
R, python, SQL, feature extraction and engineering of Wireshark capture log data, logs parsed to extract relevant RF air interface parameters. Extrapolate availability, integrity and confidentiality (AIC Triad) parameters for analyzing end to end network performance.Link parameters:  Operating  frequency:2400 -2483MHZ range within ISM band 2.4Ghz band Channel info: 79  Channels separated by 1/2 MHz Network  Topology: Point to point Modulation  coding scheme: GFSK, DQPSK, 8DPSK different for BLE or BR/EDR

## Output
The business technical goals and tradeoffs considered in characterizing the system. Results from applying venerable method used for analyzing end to end network performance.
Availability: High availability system desired
Integrity: Ensure R-R interbeat intervals transmitted without structural variation
Confidentiality: Secure Protected Health Information (PHI) transmitted over the wireless link.

## Recommendations
During normal transmission, device Bluetooth receiver sensitivity was normal, but some sensitivity drop contributed to a 36% drop in availability of the link. 
The results show that capacity utilization is less than 50%. 
Average RxLev is about -70dBm. 
The receiver experiences desensitization possibly due to hardware failure. 
Currently the system availability can  only be guaranteed at 99.759% of the time. 
Due to HIPAA confidentiality requirements, recommendation is to discontinue the transmission of personal health data (PHI) over the link that might violate HIPPA regulations.



