<p align="left">
<img src="https://i.imgur.com/t23TXuR.png" height="20%" width="20%" alt="daubert standard"/>
</p>

Introduction

Digital forensic procedures are closely complemented by incident response investigations. Incident response may be defined as an organized approach to addressing and managing the aftermath of a security breach or cyberattack – also known as an IT incident, a computer incident, or a security incident. The objective is to handle the situation in a way that limits damage and reduces recovery time and costs. Although sometimes organized and named differently according to different sources, there are typically six primary steps of an effective incident response initiative.

 

    Preparation: An incident response is not a calm and leisurely affair. Without good preparation, an incident response is going to be disorganized and has the potential to make the incident worse. A formal incident response plan is a crucial first step in preparation. Once an approved plan is in place with the appropriate staffing, ensure that the people assigned incident response duties are properly trained on the processes and procedures necessary for investigating an incident. Additionally, tools such as forensic hardware and software should be acquired and incorporated into the process.

    Detection: This is often a complex endeavor. The detection phase is the part of the incident response process where the organization first becomes aware of a set of events that possibly indicate malicious activity or constitute a threat to confidentiality, integrity, or availability. Detection can come from internal or external sources, or both.

    Analysis: In this step, personnel begin collecting evidence from systems, such as running memory, log files, network connections, and running software processes. Depending on the type of incident, this collection can take as little as a few hours to several days. The goal of the analysis step is to determine the root cause of the incident and to reconstruct the actions of the threat actor from initial compromise to detection.

    Containment: With an understanding of what the incident is and what systems are involved, the next step is the containment phase. This is when the incident response team takes measures to limit the ability of a threat actor to continue compromising network resources, communicating with command-and-control infrastructures, or exfiltrating confidential data. Containment strategies range from locking down ports and IP address on a firewall to simply removing the network cable from the back of an infected machine.

    Depending on who you ask, Containment is sometimes considered the first step in the incident response process. While this may be true in terms of overall priorities (an incident should be contained as quickly as possible), in practice, Detection, Analysis, and Containment often overlap and fold back into one another.

    Eradication and Recovery: This step is when the threat actor is removed from the impacted network. In the case of a malware infection, the incident response team may run an enhanced anti-malware solution. Other times, infected machines may be wiped and reimaged. Other activities include removing or changing compromised user accounts. If the team has identified a vulnerability that was exploited, vendor patches are applied, or software updates are made. Recovery activities are very closely aligned with those that may be found in an organization's business continuity or disaster recovery plans.

    Post-incident activity: Post-incident activity includes a complete review of all the actions taken during the incident. The team should discuss what worked and, more importantly, what did not work. It is during this phase of the process that a written report is completed. For forensic investigators, this type of documentation is critical should the incident ever wind up in court. The documentation should be detailed and show a clear chain of events with a focus on the root cause if it was determined.


In this lab, you will imitate the Analysis step of the incident response process. You will analyze a PCAP file and disk image for evidence, then prepare your findings in an incident response report. You will then continue your investigation and update your report as more evidence comes to light.



Lab Overview

SECTION 1 of this lab has three parts, which should be completed in the order specified.

 

    In the first part of the lab, you will analyze a PCAP file taken during a recent incident.

    In the second part of the lab, you will use E3 to identify forensic evidence related to the incident.

    In the third part of the lab, you will prepare an incident response report.

SECTION 2 of this lab allows you to apply what you learned in SECTION 1 with less guidance and different deliverables, as well as some expanded tasks and alternative methods. You will analyze additional evidence and update the incident response report accordingly.

 

Finally, you will explore the virtual environment on your own in SECTION 3 of this lab to answer a set of questions and challenges that allow you to use the skills you learned in the lab to conduct independent, unguided work – similar to what you will encounter in a real-world situation.



Learning Objectives

Upon completing this lab, you will be able to:

 

    Perform forensic analysis as part of an incident response investigation.

    Perform forensic analysis on a PCAP file using NetWitness Investigator.

    Perform forensic analysis on a disk image using Paraben’s E3.

    Correlate evidence from multiple sources to develop your case.

    Create an incident response report to document your findings.



Topology

This lab contains the following virtual machines. Please refer to the network topology diagram below.

 

    vWorkstation (Windows: Server 2019)

 

<img src="https://i.imgur.com/VAqa7YX.png" height="20%" width="20%" alt="daubert standard"/>



Tools and Software

The following software and/or utilities are required to complete this lab. Students are encouraged to explore the Internet to learn more about the products and tools used in this lab.

 

    NetWitness Investigator
    Paraben's E3



Deliverables

Upon completion of this lab, you are required to provide the following deliverables to your instructor:

 

SECTION 1

 

    Lab Report file including, screen captures of the following:

 

    Time Graph
    Details of the 2021-Jul-13 15:33:00 session
    Email containing FTP credentials and the associated timestamps

 

    Any additional information as directed by the lab:

 

    Completed Incident Report

 

SECTION 2

 

    Lab Report file including, screen captures of the following:

 

    Email from Dr. Evil demanding Marvin install a keylogger
    Email from Dr. Evil reminding Marvin to update the firewall and scheduler
    Registry key value associated with the keylogger and the localSPM service

 

    Any additional information as directed by the lab:

 

    Document the Author and Date values associated with the scheduled keylogger task.
    Document the port used for inbound connections to the keylogger and the name and location of the keylogger executable.
    Record the first time and last time the keylogger was started.
    Record whether Marvin interacted with or simply opened the keylogger.
    Updated Incident Report

 

SECTION 3

 

    Lab Report file including, screen captures of the following:

 

    Exfiltrated files in Marvin's Outlook database
    Email with instructions for installing additional spyware

 

    Any additional information as directed by the lab:

 

    None

<br />
<p align="center">
<img src="https://i.imgur.com/ZJsa17y.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
<img src="https://i.imgur.com/SD6Wt0O.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
<img src="https://i.imgur.com/ZK9cdBJ.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
<img src="https://i.imgur.com/kJnGQLy.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
<img src="https://i.imgur.com/NprZPj1.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
<img src="https://i.imgur.com/N36XlqY.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
<img src="https://i.imgur.com/4PUf7cH.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
<img src="https://i.imgur.com/ezKKDLM.jpeg" height="80%" width="80%" alt="forensics"/>
<br />
<br />
</p>
