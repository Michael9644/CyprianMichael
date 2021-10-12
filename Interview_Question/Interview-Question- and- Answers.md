Interview Questions by Domain
Below you will find a list of questions, grouped by specific domains. Select one question to answer. 
For each question, where appropriate, we have provided you with specific prompts to consider as you structure each section of your response. Feel free to use these prompts or your own examples.
Domain: Network Security
Question 1: Faulty Firewall
Suppose you have a firewall that's supposed to block SSH connections, but instead lets them through. How would you debug it? 
Make sure each section of your response answers the questions laid out below. 
1.	Restate the Problem:
Secure Shell (SSH) is one of the most common tools that a system administrator uses. It's essential for managing all of your servers and performing everyday tasks. In business today, information is more valuable than ever. Cybercrime is on the rise, which has led to all the top companies gearing up to protect their data. Data protection should be the top priority for all companies. This means that businesses must put in place a strong defense to prevent all kinds of cyber attacks.  One of the best defense mechanisms for network security is the Firewall Network Security. This firewall is a system designed to prevent unauthorized access to or from a private network. In this project the firewall supoose to block the SSH. Suppose you have a firewall that's supposed to block SSH connections, but instead lets them through. How would you debug it? Now the firewall instead of blocking the ssh, allows it.

2.	Provide a Concrete Example Scenario
o	In Project 1, did you allow SSH traffic to all of the VMs on your network? Yes, we did. In project 1 of my cybersecurity boot camp, we solved an almost identical problem. In that project, we deployed a virtual network containing several VMs to Azure, Adding to our defense for our network security is the firewall network security which helps to prevent unauthorized access to or from our private network.
o	Which VMs did accept SSH connections? All of them accepts SSH from my Jump box, and the Jump box accepts SSH from my computer IP address.
•	What happens if you try to connect to a VM that does not accept SSH connections? Why? It says Connection Failed/refused. This is  because  we are unable to connect to the VM on port 22.  This VM port 22, is either closed, or a rother or firewall is blocking it, or the VM is booting up and sshd is not running yet. 
3.	Explain the Solution Requirements
o	If one of your Project 1 VMs accepted SSH connections, what would you assume \the source of the error is? 
By default, Compute Engine VMs allow SSH access on port 22. If the default-allow-ssh rule is missing or misconfigured, you won't be able to connect to VMs. To resolve this issue, Check your firewall rules and re-add or reconfigure default-allow-ssh. This can also be caused by an error in our security group

o	Which general configurations would you double-check? I would check the inbound Security rules in the network security group.
o	What actions would you take to test that your new configurations are effective? We can ssh into the VM in the terminal to text if my configuration are effective.
4.	Explain the Solution Details
o	Which specific panes in the Azure UI would you look at to investigate the problem? Network security group -adjust port rules,  firewall rules and configuration settings.
o	Which specific configurations and controls would you check? I will check the ports, actions protocol and priority.
o	What would you look for, specifically? I would specifically look if the connection is denied or allowed, which port is used, if the priority of the incoming ssh inbound should be  higher than the priority that connects the ssh connection.
o	How would you attempt to connect to your VMs to test that your fix is effective? Run the ssh to the VMs with the private IP address.
5.	Identify Advantages/Disadvantages of the Solution
o	Does your solution guarantee that the Project 1 network is now "immune" to all unauthorized access? Technically, based on the solutions I offered it would to a ;large extent guarantee unauthorized access to ssh attempts, but to others I doubt. 
o	What monitoring controls might you add to ensure that you identify any suspicious authentication attempts? Detection/monitoring control to detect any suspicious authentication attempt. I can use a Checkmk, and Languardian. Install security patches, backup data online.

