# Cyber-Attack Modelling — 1

Threats can come from outside or within the organizations. Attacks can disable systems entirely or lead to prestige loss, sensitive information leaks, which would diminish consumer trust in the system provider, and they can have devastating consequences. Actually attack models say that the structure of an attack in phases. And these models provide a definition to conceptualize the different aspects of an attack. But the important point is not all attacks must complete all phases to be successful. Actually many attacks iterate recursively through the phases of an attack model.

In this series, I will talk about cyber attack models and I wanted to start with Cyber Kill Chain.
## Cyber Kill Chain

In fact “Kill Chain” is a military term used to describe the phases of an attack that the process is described as find, fix, track, target, engage, assess (F2T2EA) but scientists in Lockheed Martin used this concept to develop the Cyber kill chain.

Regardless, it has become an almost standard framework which others have altered or extended in different ways. Some people love it and some do not. So even if people criticize it, generally cyber kill chain identifies the steps of an attack from reconnaissance to controlling the systems with malware.
https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html

Every chain depends on the other. So if one chain fails, all kill chain will be unsuccessful. 

#### **Chain is no stronger than its weakest link**
  
Lockheed Martin’s cyber kill chain breaks down an external-originating cyber attack into 7 distinct steps:
### Reconnaissance

Reconnaissance, the first phase of an attack. In this chain, the attacker picks a target, researches it, and looks for vulnerabilities.

This phase cannot always be detected, but in order to protect yourself, you can make the attacker’s job harder.. Perform your own recon by monitoring various social media outlets etc. and eliminate valuable sources of information when possible. You should conduct a reconnaissance phase for yourself before the intruder.

> Reconnaissance phase can be detected by web analytics and denied by Firewall and ACL.

Some indicator example for Reconnaissance Phase are:
• Recipient List
• Benign File: idno.pdf
Weaponization

The intruder develops malware designed to exploit the vulnerability. This malware can be injected into different files such as PDF, photos etc.

The classic risk equation is:

**Risk = Threat * vulnerability * Impact**

If you know where your vulnerabilities are, you can also guess what an attacker may target and how they may attempt to exploit a weakness. Therefore, you should reduce the number of types of vulnerabilities in your system and make the weaponization phase harder for intruders to protect yourself.

>Weaponization phase can be detected by NIDS and denied by NIPS.

Some indicator example for Weaponization Phase:
- Trivial encryption algorithm: Key1 

### Delivery

If an attacker could manage to come up to this stage, he/she transmits the malware that he/she developed in the weaponization phase, via a phishing email or another channel. Maybe intruders can use compound methods but most of the time, the human factor is at the center of these types of attacks.

Consequently, education has to be a key part of any information security program, however since humans are peccant, using humans will always be an effective method to deliver weapons to targets until we can teach machines to protect us from ourselves.

> Delivery phase can be detected by vigilant users, denied by proxy filter, and disrupted by an AV.

Some indicator example for Delivery Phase:
- username@company.com
- IP Address : x.x.x.x

### Exploitation

The malware begins executing on the target system, such as the exploit running on the system.

With the purpose of protecting yourself, systems that are being used in your company should always be updated. It should always be checked that every system has an anti-virus running and enabled to make the them far more secure against any type of attacks.

> Exploitation phase can be detected by HIDS, denied by patches and disrupted by DEP

Some indicator example for Exploitation Phase:
- CVE-2013–0432
- Shellcode

### Installation

In Installation phase, malware installs a backdoor or another entry accessible for the attacker. Not all attacks require malware such as CEO fraud attack or harvesting login credentials.

For the sake of your company, there should always be a trained and intelligent workforce. Also your employees should ensure they are using secure devices that are updated, and have anti-virus enabled, which would detect many malware installation attempts. Who could be a better candidate than the man using the system every day to detect abnormal behavior in their system? Hence, people should use “human firewall” and as leverage the “human sensor”.

> Installation phase can be detected by HIDS, denied by chroot jail and disrupted by AV

Some indicator example for Installation Phase:
- C:\..\..\EXPLORE.hip
- C:\..\..\fssm32.exe

### Command and Control

A command-and-control [C&C] server is a computer controlled by an attacker or cybercriminal which is used to send commands to systems compromised by malware and receive stolen data from a target network. When intruder gains system control, he/she connects systems to C&C for provide persistence in the system. As a result, the intruder gains persistent access to the victim’s systems/network.

> Command and Control phase, can be detected by NIDS, denied by Firewall ACL, disrupted by NIPS, and deceived by DNS redirection

Some indicator example for Command and Control Phase:
- 100.x.x.12

### Actions on Objective

When the intruder establishes access to the organization, he/she can perform every action to achieve their aims. Motivations greatly vary depending on the threat actor. It may include political, financial, or military gain, so it is very difficult to guess what those actions are going to be. Therefore, in this phase, intruder initiates end goal actions, such as data theft, data corruption, or data destruction.

In order to keep yourself protected, critical information should not be kept unprotected in accessible places.

> Actions on Objective phase can be detected by Audit logs, deceived by honeypots and degraded by quality of service.

#### References:

- https://medium.com/@winstark_212/cyber-kill-chain-and-mitre-att-ck-c67ab9c59646

- https://www.lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/Gaining_the_Advantage_Cyber_Kill_Chain.pdf

[Go to Dashboard](https://mergenhan.github.io/index.html)
