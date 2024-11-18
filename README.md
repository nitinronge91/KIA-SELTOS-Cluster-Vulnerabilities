# KIA-SELTOS-Cluster-Vulnerabilities
This repository documents the vulnerabilities identified during penetration testing of the [KIA SELTOS](https://en.wikipedia.org/wiki/Kia_Seltos) (Indian Varient) vehicle cluster system. It provides a comprehensive record of findings, their potential impact on security, and recommended remediation steps. The aim is to enhance the security posture of automotive systems through detailed vulnerability documentation and actionable insights.This engaement was completely based on black box testing approach.

Product details are as follows:

Instrument Cluster KIA Seltos - SW : 1.0, HW:1.0, Date of Manufacturer: 16 June 2023

<img width="1139" alt="KIA_Cluster_Img" src="https://github.com/user-attachments/assets/2db7d9a8-1da6-4c84-bf84-25ecf9383970">

## Initial Reconnisance
As we followed black box PEN test approach, We need to tear down the cluster for intital reconissance.  As we removed the cluster from vehicle, Power Pin connections we got from vehicle.
Now next step was to find CAN pins from socket!


## Vulnerabilities Reported

 [Odometer Manipulation for KIA SELTOS CVE-2024-51074](https://github.com/nitinronge91/KIA-SELTOS-Cluster-Vulnerabilities/blob/636bec2787472aa1a68539806ab8c83697131c8e/CVE/Odometer%20Manipulation%20For%20KIA%20SELTOS%20CVE-2024-51074)

[ Control CAN communication for KIA SELTOS Cluster CVE-2024-51073](https://github.com/nitinronge91/KIA-SELTOS-Cluster-Vulnerabilities/blob/b61106ffaf12a8eb9c78607b0f5e7821d56cd964/CVE/Control%20CAN%20communication%20for%20KIA%20SELTOS%20Cluster%20CVE-2024-51073)

 [ Denial OF service via ECU Reset service for KIA SELTOS Cluster CVE-2024-51072](https://github.com/nitinronge91/KIA-SELTOS-Cluster-Vulnerabilities/blob/b61106ffaf12a8eb9c78607b0f5e7821d56cd964/CVE/Denial%20of%20Service%20via%20ECU%20Reset%20Service%20For%20KIA%20SELTOS%20CVE-2024-51072)

 

