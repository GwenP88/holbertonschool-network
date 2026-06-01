<p align="center">
  <img src="./assets/banner.jpeg" alt="holbertonschool-network Banner" height="500">
</p>

# Networking basics #1

> Because knowing what localhost *really* is might just save your network (and your sanity).

---

## 📝 Description

This project is part of the Holberton School curriculum and focuses on the fundamentals of networking in a Linux environment. I explore core network concepts such as IP addressing, hostname resolution, and port communication — all through Bash scripting. The tasks involve manipulating the `/etc/hosts` file to change how the system resolves domain names, listing active network interfaces, and creating a script that listens on a port. It's the kind of low-level networking knowledge that makes you feel like a wizard... or at least someone who can confidently explain why `ping localhost` matters.

---

## 🎯 Learning Objectives

At the end of this project, I am able to explain, without the help of Google, what `localhost` and `127.0.0.1` represent and why they point to the same machine. I understand what `0.0.0.0` means in the context of network binding and how it differs from a specific IP address. I know the role of the `/etc/hosts` file and how it can override DNS resolution locally. Finally, I am able to display all active network interfaces on a machine using the appropriate system commands.

---

## 🛠️ Technologies Used

This project is written entirely in Bash and runs on Ubuntu 22.04 LTS. I use standard Unix networking tools such as `ip`, `hostname`, and `nc` (netcat). All scripts are validated with ShellCheck (version 0.7.0) to ensure clean, portable, and error-free shell code. No external libraries or frameworks required — just the shell and its built-in power.

---

## ⚙️ Requirements

- **OS:** Ubuntu 22.04 LTS
- **Allowed editors:** `vi`, `vim`, `emacs`
- All files must end with a new line
- The first line of all Bash scripts must be exactly: `#!/usr/bin/env bash`
- The second line of all Bash scripts must be a comment explaining what the script does
- All Bash script files must be executable
- Scripts must pass `Shellcheck` (version `0.7.0` via `apt-get`) without any errors
- A `README.md` file at the root of the project is mandatory

---

## 🚀 Installation

```bash
git clone https://github.com/GwenP88/holbertonschool-network.git
cd holbertonschool-network/basics_1
```

---

## ▶️ Usage / Execution

All Bash scripts can be executed in two ways:

### 1. Direct execution
Make the file executable and run it directly:
```bash
chmod +x filename
./filename
```

### 2. With sudo (when system-level changes are required)
Some scripts modify system files and require elevated privileges:
```bash
sudo ./filename
```

---

## 📊 Project Progress

<p align="center">
<img src="assets/progress_barre_100.gif" alt="Mandatory tasks progress" width="80%">
</p>

<p align="center">
<sub>Mandatory tasks completion: 100%</sub>
</p>

---

## ✨ Features

### Task 0 - Change your home IP

- **Status:** Mandatory
- **Objective:** Write a Bash script that reconfigures DNS resolution on an Ubuntu server by modifying the `/etc/hosts` file.
- **Constraint:** `localhost` must resolve to `127.0.0.2` and `facebook.com` must resolve to `8.8.8.8`. Script must be run with `sudo`. ⚠️ Remember to revert `localhost` to `127.0.0.1` after testing — otherwise things will start breaking in entertaining but frustrating ways.
- **Expected behavior:** After running the script, `ping localhost` returns `127.0.0.2` and `ping facebook.com` returns `8.8.8.8`.

**Files:** `0-change_your_home_IP`

---

### Task 1 - Show attached IPs

- **Status:** Mandatory
- **Objective:** Write a Bash script that displays all active IPv4 IP addresses on the machine it is executed on.
- **Constraint:** The output must list all active IPv4 addresses, one per line. Results will vary depending on the machine.
- **Expected behavior:** Running the script outputs all active IPv4 addresses, including the loopback address `127.0.0.1`.

**Files:** `1-show_attached_IPs`

---

### Task 2 - Port listening on localhost

- **Status:** Mandatory
- **Objective:** Write a Bash script that listens on port `98` on `localhost`, allowing incoming text connections via `telnet`.
- **Constraint:** Must be run with `sudo`. The script opens a socket on port 98 and displays any text received from a connecting client.
- **Expected behavior:** In one terminal, the script listens silently. In a second terminal, connecting via `telnet localhost 98` and typing text causes that text to appear live in the first terminal. Useful for debugging socket connections and firewall rules — or just for impressing your classmates.

**Files:** `2-port_listening_on_localhost`

---

## 🤝 Contributions & Acknowledgements

A huge thank you to the Holberton School staff and peers who helped me navigate the wonderful (and sometimes maddening) world of networking. Special appreciation to everyone who reminded me that `127.0.0.1` and `localhost` are *supposed* to be the same thing — until they're not. 🙃

---

## 👤 Author

**Gwenaelle PICHOT**
- Student at Holberton School
- Track: holbertonschool-network
- Project: Networking basics #1