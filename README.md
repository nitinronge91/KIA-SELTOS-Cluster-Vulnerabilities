# KIA-SELTOS-Vehicle-Cluster-Vulnerabilities
This repository documents the vulnerabilities identified during penetration testing of the [KIA SELTOS](https://en.wikipedia.org/wiki/Kia_Seltos) (Indian Varient) vehicle cluster system. It provides a comprehensive record of findings, their potential impact on security, and recommended remediation steps. The aim is to enhance the security posture of automotive systems through detailed vulnerability documentation and actionable insights.This engaement was completely based on black box testing approach.
we suspect that these vulnerabilities are present in majority of the KIA vehicles in Indian market .

Product details are as follows:

**Instrument Cluster KIA Seltos - SW : 1.0, HW:1.0, Date of Manufacturer: 16 June 2023**

<img width="1133" alt="386580515-2db7d9a8-1da6-4c84-bf84-25ecf9383970" src="https://github.com/user-attachments/assets/efd75017-2070-448b-8d5b-b03c485a6209">

![](https://github.com/nitinronge91/KIA-SELTOS-Cluster-Vulnerabilities/blob/198ca874bdaa652c88cb27cdaefbd4cace707c32/Cluster_KIA.gif)

##  Reconnisance
We employed a black-box penetration testing approach for this assessment. To begin the initial  reconnisance, it was necessary to disassemble the instrument cluster from the vehicle. Upon removal, we identified the power supply pin connections using the vehicle's wiring system.

The next step involved identifying the CAN communication pins on the cluster’s connector to access and analyze the In-Vehicle Network (IVN). Referring to the System-on-Chip (SoC) datasheet, we determined that the cluster was equipped with two CAN channels for communication. Using the controller’s pinout, we traced the connectivity to the connector pins and successfully identified the CAN_H and CAN_L pins, as shown in the accompanying diagram.

We then configured a CAN interface on a PC to monitor traffic on both identified channels. Upon establishing the setup, we observed active CAN messages on one of the channels, indicating live communication on the CAN bus.
This discovery served as a critical entry point for further testing. Leveraging the CAN and Unified Diagnostic Services (UDS) protocols, we proceeded to exploit the cluster’s communication network for in-depth analysis.

![image](https://github.com/user-attachments/assets/d37bec7a-34c5-4a93-af0a-d8e679df475a)




## Vulnerabilities Reported

 [Odometer manipulation(increament) for KIA seltos vehicle cluster CVE-2024-51074](https://github.com/nitinronge91/KIA-SELTOS-Cluster-Vulnerabilities/blob/0446f6fe6299eb39310e996c73d5513e70d76353/CVE/Odometer%20Manipulation(Increase)%20for%20KIA%20SELTOS%20Cluster%20CVE-2024-51074.md)

 [Control CAN communication for KIA seltos vehicle cluster CVE-2024-51073](https://github.com/nitinronge91/KIA-SELTOS-Cluster-Vulnerabilities/blob/3755e3f692dce5b1ab06de2d04a2433c907ab21c/CVE/Control%20CAN%20communication%20for%20KIA%20SELTOS%20Cluster%20CVE-2024-51073.md)

 [Denial Of service via ECU Reset service For KIA Sletos vehicle Cluster CVE-2024-50172](https://github.com/nitinronge91/KIA-SELTOS-Cluster-Vulnerabilities/blob/628b1550f0093f79380929074b6a5e6ca6f2d04b/CVE/Denial%20of%20Service%20via%20ECU%20Reset%20Service%20For%20KIA%20SELTOS%20CVE-2024-51072.md)

     
## Authors:
   Nitin Ronge(www.linkedin.com/in/nitin-ronge)
   
   Shakir zari(www.linkedin.com/in/shakir-zari)
  
   Anand Yadav(www.linkedin.com/in/anandyadav6962)
   

 

