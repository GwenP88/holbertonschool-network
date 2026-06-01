<p align="center">
  <img src="./assets/banner.jpeg" alt="holbertonschool-network Banner" height="500">
</p>

# holbertonschool-network

> From OSI layers to live port listening — a hands-on journey through the fundamentals of computer networking.

---

## 📄 Description

This repository gathers my Holberton School projects on computer networking. Through theory-based question files and Bash scripting tasks, I progressively built a solid understanding of how networks work — from abstract models like OSI down to very concrete things like pinging a server or making a port listen on localhost. Each directory corresponds to a standalone project with its own objectives, constraints, and deliverables. No prior networking wizardry required at the start; plenty gained by the end.

---

## 🎯 Learning Objectives

The main goal of this repository is to build a working understanding of computer networking from the ground up. Across both projects, I learned to explain the OSI model and its 7 layers, distinguish between LAN, WAN, and the Internet, understand IP and MAC addressing, differentiate TCP from UDP, work with port numbers (SSH: 22, HTTP: 80, HTTPS: 443), use ICMP via `ping` to check network availability, manipulate the `/etc/hosts` file to control local DNS resolution, display active network interfaces, and create a script that listens on a port in real time.

---

## 📁 Repository Structure

```bash
holbertonschool-network/
├── basics_0/
├── basics_1/
└── README.md
```

---

## ✨ Projects / Contents

### basics_0 — Networking basics #0
- Introduction to the OSI model, LAN/WAN/Internet, IP and MAC addresses, TCP/UDP protocols, port numbers, and ICMP
- Includes multiple choice answer files and two Bash scripts: one to list listening ports, one to ping a host
- Main technologies: Bash, `netstat`, `ping`, Ubuntu 22.04 LTS

### basics_1 — Networking basics #1
- Deeper dive into IP addressing, localhost, `/etc/hosts` manipulation, and port listening via `nc`
- Includes Bash scripts to change DNS resolution, display active IPs, and open a listening socket on port 98
- Main technologies: Bash, `ip`, `nc` (netcat), Ubuntu 22.04 LTS

---

## 🛠️ Technologies Used

- **Bash** — all tasks are implemented as shell scripts
- **Ubuntu 22.04 LTS** — target execution environment
- **ShellCheck** — used to validate all scripts (version 0.7.0)
- **Standard Unix networking tools** — `netstat`, `ping`, `ip`, `nc`

---

## ⚙️ Prerequisites

- OS: Ubuntu 22.04 LTS
- Bash shell
- ShellCheck installed (`apt-get install shellcheck`)
- Some scripts require `sudo` privileges (e.g. modifying `/etc/hosts` or binding to a port)
- Allowed editors: `vi`, `vim`, `emacs`

---

## ▶️ Usage

```bash
git clone https://github.com/GwenP88/holbertonschool-network.git
cd holbertonschool-network
```

Each project lives in its own directory. Navigate into the one you want to explore:

```bash
cd basics_0   # or basics_1
```

For answer files, simply read the content:
```bash
cat 0-OSI_model
```

For Bash scripts, make them executable and run:
```bash
chmod +x script_name
./script_name        # or: sudo ./script_name
```

Refer to each project's own `README.md` for detailed usage instructions and task descriptions.

---

## 🤝 Contributions & Acknowledgements

Big thanks to the **Holberton School** curriculum team for designing projects that actually make networking feel approachable. Thanks also to my peers for the debugging sessions, the well-placed hints, and the collective suffering over `localhost` resolving to the wrong address. You know who you are. 🙏

---

## 👤 Author

**Gwenaelle PICHOT**
- Student at Holberton School
- Repository: holbertonschool-network