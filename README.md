
The objective of this project is to set up a basic home cybersecurity lab to gain hands-on experience in various cybersecurity concepts and tools. The lab is set up using VMware, which enables the creation of multiple virtual machines (VMs) to simulate a real-world environment. 

## ** Project Goals:**

1. To create a virtualized environment that simulates a SOC analyst's work environment.
2. To configure and secure an Ubuntu server and a Windows machine.
3. To disable Windows Defender on the Windows machine using Group Policy and Registry settings.
4. To use Sliver to create a C2 payload and download it onto the Windows machine.
5. To implement Sysmon and Limacharlie to monitor and analyze telemetry, process, and network activity of malware.
6. To conduct hash analysis to identify and understand the malicious behavior of the malware.
7. To develop and implement custom detection rules to proactively detect and mitigate malicious activity, including ransomware attacks.
8. To demonstrate proficiency in using command-line interfaces to connect to the Windows machine and terminate parent activity during a simulated ransomware attack.

## **Methodology:**

1. Setup: VMware was used to set up the lab environment. Two VMs were created, an Ubuntu server, and a Windows 10 machine.
2. Disabling Windows Defender: Windows Defender was disabled using the Group Policy Editor and the Registry Editor. This was done in both normal and safe mode to ensure complete disabling of the antivirus tool.
3. Improved payload delivery and connectivity: The IP address of the Ubuntu Server was changed to a static one to ensure consistency while creating and delivering the payload. SSH was also enabled on the Ubuntu Server to easily access it from the host machine.
4. Installation of Sliver: Sliver was installed on the Ubuntu server and a C2 payload was created to control the Windows 10 machine.
5. Setting up Sysmon: Sysmon was installed in the Windows 10 machine to monitor its activity and log events related to process creation, network connections, and more.
6. Setting up Limacharlie: Limacharlie was installed in the Windows 10 machine to monitor its activity and detect malicious behavior.
7. Downloading and running the C2 payload: A temporary server was created using Python in Ubuntu, and it was used to download the C2 payload in Windows. The payload was then run in Windows.
8. Inspecting the telemetry data in Limacharlie: The telemetry data generated by Limacharlie was analyzed to detect any malicious activity in the Windows 10 machine. The sensors, processes, and network connections were monitored for any suspicious activity. The hash value of the payload was also inspected using VirusTotal to determine if it was a known malware.
9. Blocking an attack: A ransomware attack was simulated by attempting to delete the volume shadow copies in Windows from attack machine. This action was detected by Limacharlie, and a detection rule was created to terminate the parent activity, which would be the ransomware payload or lateral movement.


## **Technical Skills Acquired**

- Experience with VMware and virtual machines
- Knowledge of Group Policy Editor and Registry Editor
- Experience with Sliver, an essential tool in red team operations
- Experience with Sysmon, an essential tool for system monitoring
- Experience with Limacharlie, an endpoint detection and response tool
- Experience with Python
- Knowledge of hash analysis and detection rules development.
- Experience with detecting and blocking attacks
- Familiarity with command-line interfaces.

## **Conclusion**

The home cybersecurity lab project was a comprehensive learning experience that helped me gain valuable knowledge and practical experience in various cybersecurity concepts and tools. Through this project, I was able to set up a virtualized environment that simulated a SOC analyst's work environment, configure and secure an Ubuntu server and a Windows machine, and disable Windows Defender on the Windows machine using Group Policy and Registry settings.

I also learned how to use Sliver to create a C2 payload and how to implement Sysmon and Limacharlie to monitor and analyze telemetry, process, and network activity of malware. The project allowed me to conduct hash analysis to identify and understand the malicious behavior of the malware and to develop and implement custom detection rules to proactively detect and mitigate malicious activity, including ransomware attacks.

Overall, the project provided a practical and hands-on learning experience in cybersecurity concepts and tools, which will be beneficial in real-world cybersecurity operations. More attack scenarios and detection
