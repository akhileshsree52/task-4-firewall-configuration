# Task 4: Setup and Use a Firewall (UFW)

## Objective
Configure and test basic firewall rules to allow or block network traffic using UFW on Linux.

## Tools Used
- Linux (Ubuntu/Kali)
- UFW (Uncomplicated Firewall)

## Steps Performed

### 1. Enabled UFW
Checked and enabled the firewall using:
sudo ufw enable

### 2. Listed Current Rules
sudo ufw status verbose

### 3. Blocked Telnet (Port 23)
sudo ufw deny 23

Reason: Telnet transmits data in plain text and is insecure.

### 4. Tested the Rule
Attempted to connect using:
telnet localhost 23

Connection was refused, confirming the rule worked.

### 5. Allowed SSH (Port 22)
sudo ufw allow 22

This ensures secure remote access.

### 6. Removed Test Rule
sudo ufw delete deny 23

Restored firewall to original state.

## Outcome
- Learned basic firewall rule management
- Understood inbound traffic filtering
- Gained hands-on experience with UFW

## Screenshots
All relevant screenshots are available in the screenshots folder.
