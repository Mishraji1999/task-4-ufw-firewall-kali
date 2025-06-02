 Task 4 - UFW Firewall Configuration on Kali Linux
🎯 Objective
To configure and test basic firewall rules using UFW (Uncomplicated Firewall) on Kali Linux.
This task demonstrates how to block, allow, and manage inbound traffic based on specific ports.

🛠 Commands Used & Output Explanation
Step 1: Enable UFW
sudo ufw enable

Step 2: Check Current Rules (Verbose Mode)
sudo ufw status verbose
Displays the current UFW status, default policy, and any active rules.

Step 3: Block Inbound Traffic on Port 23 (Telnet)
sudo ufw deny 23
Telnet is insecure. Blocking it protects from unencrypted login attacks.

Step 4: Allow Inbound Traffic on Port 22 (SSH)
sudo ufw allow 22
Allows SSH remote access securely.

Step 5: Remove Test Rule (Telnet Block)
sudo ufw delete deny 23
Removes the port 23 block, restoring firewall state.

Step 6: View Numbered Rules (For Reference)
sudo ufw status numbered
Shows rules with numbers, useful to delete by index.

💡 Key Concepts Learned
UFW is a simple front-end for iptables.

Blocking Telnet improves security.

Port-specific rules secure inbound traffic without blocking outbound.

🔐 Why Block Port 23 (Telnet)?
Telnet sends usernames and passwords in plain text, which can be intercepted easily. Blocking it enhances system security.

📸 Screenshot
Screenshot of all steps is saved in /screenshots/Task4-ufw.png.

✅ Task Completed By:
Name: Suraj Mishra
Platform: Kali Linux (Minimal)
Tool Used: UFW

