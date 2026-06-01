<p align="center">
  <img src="./assets/banner.png" alt="holbertonschool-network Banner">
</p>

# Networking basics #0

> Because understanding how the internet works is way more interesting than just complaining about the Wi-Fi.

---

## 📝 Description

This project is an introduction to the fundamentals of computer networking. Through a series of conceptual questions and Bash scripting tasks, I explore the OSI model, the differences between LAN and WAN, the role of IP and MAC addresses, TCP and UDP protocols, port numbers, and the ICMP protocol. By the end, I have a solid foundation to understand how devices communicate over a network — and enough knowledge to impress at a dinner party (or at least troubleshoot my own connection).

---

## 🎯 Learning Objectives

At the end of this project, I am able to explain the OSI model, describing what it is, how many layers it has, and how it is organized from the physical transmission layer up to the application layer. I understand what a LAN is, its typical usage for connecting local devices, and its limited geographical size. I can also explain what a WAN is, how it connects multiple LANs across larger distances, and its role in wide-area communication. I am able to describe what the Internet is, what an IP address represents, the difference between public and private IP addresses, what `localhost` refers to, what a subnet is, and why IPv6 was created to address the exhaustion of IPv4 addresses. Regarding TCP/UDP, I can identify the two main data transfer protocols used at the transport layer of the OSI model, explain the key difference between them (reliability vs. speed), define what a port is, recall the port numbers for SSH (22), HTTP (80), and HTTPS (443), and identify `ping` (ICMP) as the standard tool used to check network device availability.

---

## 🛠️ Technologies Used

This project is built entirely with **Bash** scripting, interpreted on **Ubuntu 22.04 LTS**. Scripts are written to be compliant with **shellcheck** and follow strict formatting rules. The networking concepts explored rely on standard Unix tools such as `netstat` and `ping`, both part of the default Linux networking toolkit.

---

## ⚙️ Requirements

- **OS:** Ubuntu 22.04 LTS
- **Shell:** Bash
- **Allowed editors:** `vi`, `vim`, `emacs`
- All files must end with a new line
- The first line of all Bash scripts must be exactly: `#!/usr/bin/env bash`
- The second line of all Bash scripts must be a comment explaining what the script does
- All Bash script files must be executable
- All Bash scripts must pass `shellcheck` without any error
- A `README.md` file at the root of the project folder is mandatory
- For multiple choice answer files: write only the number of the correct answer, one per line

---

## 🚀 Installation

```bash
git clone https://github.com/GwenP88/holbertonschool-network.git
cd holbertonschool-network/basics_0
```

---

## ▶️ Usage / Execution

### 1. Answer files (multiple choice tasks)
These files simply contain the number(s) of the correct answer(s):
```bash
cat 0-OSI_model
```

### 2. Bash scripts
Make the file executable and run it directly:
```bash
chmod +x 4-TCP_and_UDP_ports
sudo ./4-TCP_and_UDP_ports
```

Or for the ping script with an IP argument:
```bash
chmod +x 5-is_the_host_on_the_network
./5-is_the_host_on_the_network 8.8.8.8
```

---

## 📊 Project Progress

<p align="center">
<img src="assets/progress_barre_100.gif" alt="Mandatory tasks progress" width="80%">
</p>

<p align="center">
<sub>Mandatory tasks completion: 100% </sub>
</p>

---

## ✨ Features

### Task 0 - OSI model

- **Status:** Mandatory
- **Objective:** Understand what the OSI model is and how it is organized across its 7 layers, from physical transmission to application-level communication.
- **Constraint:** Answer file only — select the correct answers from the provided multiple choice questions.
- **Expected behavior:** The file contains the numbers corresponding to the correct answers, one per line.

**Files:** `0-OSI_model`

---

### Task 1 - Types of network

- **Status:** Mandatory
- **Objective:** Distinguish between LAN, WAN, and Internet network types based on their typical usage and geographical coverage.
- **Constraint:** Answer file only — select the correct answers from the provided multiple choice questions.
- **Expected behavior:** The file contains the numbers corresponding to the correct answers, one per line.

**Files:** `1-types_of_network`

---

### Task 2 - MAC and IP address

- **Status:** Mandatory
- **Objective:** Understand the role of MAC addresses as unique hardware identifiers and IP addresses as logical network identifiers.
- **Constraint:** Answer file only — select the correct answers from the provided multiple choice questions.
- **Expected behavior:** The file contains the numbers corresponding to the correct answers, one per line.

**Files:** `2-MAC_and_IP_address`

---

### Task 3 - UDP and TCP

- **Status:** Mandatory
- **Objective:** Differentiate between TCP (reliable, slower) and UDP (fast, potentially lossy) and understand how the TCP handshake confirmation mechanism works.
- **Constraint:** Answer file only — select the correct answers from the provided multiple choice questions.
- **Expected behavior:** The file contains the numbers corresponding to the correct answers, one per line.

**Files:** `3-UDP_and_TCP`

---

### Task 4 - TCP and UDP ports

- **Status:** Mandatory
- **Objective:** Write a Bash script that displays all currently listening ports along with the PID and name of the associated program.
- **Constraint:** The script must use `netstat`, show only listening sockets, and display PID/program names. Must pass `shellcheck`.
- **Expected behavior:** Running `sudo ./4-TCP_and_UDP_ports` outputs a formatted list of active listening connections including protocol, address, state, and program name.

**Files:** `4-TCP_and_UDP_ports`

---

### Task 5 - Is the host on the network

- **Status:** Mandatory
- **Objective:** Write a Bash script that pings a given IP address 5 times using ICMP to check network availability.
- **Constraint:** The script must accept an IP address as an argument and display a usage message if no argument is provided. Must pass `shellcheck`.
- **Expected behavior:** Running `./5-is_the_host_on_the_network 8.8.8.8` sends 5 ICMP pings and displays the results. Running it without an argument prints `Usage: 5-is_the_host_on_the_network {IP_ADDRESS}`.

**Files:** `5-is_the_host_on_the_network`

---

## 🤝 Contributions & Acknowledgements

A big thank you to the **Holberton School** team for the project structure and resources. Special mention to the `ping` command, which taught me more about my own network than I ever wanted to know. No Stack Overflow tabs were harmed in the making of this project. 🙏

---

## 👤 Author

**Gwenaelle PICHOT**
- Student at Holberton School
- Track: holbertonschool-network
- Project: Networking basics #0