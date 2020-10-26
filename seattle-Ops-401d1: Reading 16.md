                                                  Threat Analysis, Cyber Kill-Chain, and Stuxnet

Cybersecurity Kill Chain is defined as a 7 , sequential, step approach an attacker takes to complete a successful attack. It was developed by Lockheed Martin. The step are as follows:

1.	Reconnaissance
2.	Weaponization
3.	Delivery
4.	Exploitation
5.	Installation
6.	Command and Control
7.	Actions on Objectives

If one or more of the 7 steps is broken, the attack will be disrupted, resulting in a failed attack.
In reconnaissance, the attacker tries to gather enough information about the victim in either a passive or active stage. 

                                                                Reconnaissance

In passive reconnaissance, the attacker uses public sources such Google, Facebook, WHOIS, ARIN registrations, Google, Shodan, Job Listings and company website to gather information about the victim. 
The attacker then proceed to interact with the organization with the users credentials. She/he uses tools such nMap among others to gain access to vital information. 
Before utilizing defense tools and techniques to foil this kind of attacks, users should be encouraged to limit sharing important information publicly.   

                                                                 Weaponization

Weaponization, which is the second step in the seven steps, is when the attacker utilizes the information she/he acquired from the user to exploit the system. 
In this stage, techniques such patch management should be implemented to keep the system up to date on patches in order to prevent unauthorized intrusion.
Once our system is attacked, a post infection tool, like a sandbox or an EDR, will help us detect zero day threats that are preventive measures didn’t detect.

                                                                   Delivery

When the attacker selects the weapon to use for the attack, she/he then moves to the Delivery stage where the attacker tries one or multiple avenues to deliver the weapon. Some delivery examples are:  Websites (malicious or clean, social media, user input, email, and USB’s. Besides awareness campaign, support staff may use tools and techniques such as DKIM and SPF email authentication methods to detect spoofed emails. The may also use Web filtering to prevent users from accessing questionable or known bad sites, disabling USB,  DNS filtering to name a few.  

                                                                  Exploitation

The exploitation stage is where the attack is executed. This means we have failed to keep the weapon away from our environment, and the only thing left is for the attacker to pull the trigger. 
The actual exploit could come in different forms such as a buffer overflow, a SQL injection, other malware the systems anit-virus (AV) could not detected or many others. 
Once an attack is executed, there’s very little we can do except to try to minimize the damage.  We may utilize tools such as:  
•	DEP (Data Execution Prevention) is a software and hardware feature which attempts to prevent the execution of code in memory where it doesn’t belong.  
•	Anti-Exploit is a feature on some AV solutions that monitor known applications for unusual calls to memory.
•	Both of these techniques act as the last line of defense against common exploit attempts
The reality is when an attacker gets to this point you’re relying on post-infection tools like a sandbox, EDR or a SIEM to find indicators of compromise (IoC). A Sandbox has some prevention capabilities depending on the scenario but for most network environments, you have what’s called “Patient Zero”. Patient Zero refers to the first time an unknown file is seen on the network. 

                                                                  Installation

The Installation and exploitation phase go hand in hand. A successful exploit allows me to  inject a payload that will give me a better level of access to accomplish the mission. From an attackers perspective, gaining better access allows me to control the victim at any point in the future, even after a system has been patched.  
Some common payloads and techniques during this stage involve:
•	DLL hijacking
•	Injecting Meterpreter or other similar payloads
•	Installing Remote Access Tools (or RAT)
•	Registry changes to make my program automatically start up
•	Executing Powershell in fileless attacks
Once an attacker has gotten this far into the system, very limited protective tools exist. In Linux we can use Chroot jail to isolate processes from the rest of the system to limit the amount of a data the malicious file has access to and Windows systems can disable PowerShell on all systems that do not require it. But not all is doom, fortunately, we can use a good EDR solution should flag any new unauthorized program that was installed, as well as detect any changes to registry and system process.

                                                                Command and Control

At this stage, the system has been completely compromised and in control of the attacker. If they completed the previous stage correctly, their access is persistent – even if you reboot or patch the vulnerability. At this point the defensive tactics in the system are going to limit what they can control and detect unusual activity. 

Network Segmentation will make it harder for the attacker to move laterally, and easier to detect using audit logs. A micro segmentation through a “Zero trust security” model, may work better. This would essentially leave the infected user completely isolated on that port until they can verify their machine is clean and have been authenticated. 

                                                                Actions on Objective

With the machine now infected and the attacker in full control, they can now execute the action to achieve their objective. The action is predicated by the motivation of the attacker, so understanding the type of attacker that could be targeting your organization is crucial. Attackers could be motivated by: financial reasons, political, Nation-State, Malicious Insiders, or simply moving laterally to go after other systems on the network.  
If the goal is data exfiltration, we can look into tools that prevent data from moving off the endpoint or server. On the endpoint, tools like a DLP or UBA solution have complimentary features to detect and prevent specific files from moving off the network. The problem is, if an attacker has already gained access into your system – doing something as simple as screenshotting a protected document may not be detected by any of these tools. 
 
                                                                The CISO Perspective
 
The kill chain is more than just a model for how an attack executed, it is a blueprint for building a good cybersecurity program. By using multiple layers of security throughout each phase, the support team can make it more and more challenging for the attacker to be successful – and that by itself is a victory because so many attacks are opportunistic in nature. 

