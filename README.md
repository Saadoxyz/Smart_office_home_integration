
# 🏠🏢 Smart Office + Home Integration Project — Cisco Packet Tracer

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=00D4AA&center=true&vCenter=true&width=800&lines=Smart+Office+%2B+Home+Device+Network;Cisco+Packet+Tracer+Inter-VLAN+Project;IoT+Integration+%7C+FTP+%7C+Email+%7C+Web+%7C+ACL+Security" alt="Typing SVG" />
</div>

<div align="center">

![Cisco](https://img.shields.io/badge/Platform-Cisco%20Packet%20Tracer-00A8E8?style=for-the-badge&logo=cisco&logoColor=white)
![Level](https://img.shields.io/badge/Level-Beginner%20to%20Intermediate-yellowgreen?style=for-the-badge)
![IoT](https://img.shields.io/badge/IoT-Simulation%20Ready-orange?style=for-the-badge)
![VLAN](https://img.shields.io/badge/VLAN-Enabled-purple?style=for-the-badge)
![Routing](https://img.shields.io/badge/Inter--VLAN-Routing-green?style=for-the-badge)
![ACLs](https://img.shields.io/badge/ACLs-Implemented-critical?style=for-the-badge)

</div>

---

## 🌐 Project Overview

This Cisco Packet Tracer project simulates a **Smart Office Network** where **Home IoT devices** securely connect to **Office infrastructure** via VLAN segmentation and Inter-VLAN Routing.

> 🔒 Communication between networks is strictly controlled using **Access Control Lists (ACLs)**.

---

## 🧩 Key Components

- 🔌 **2 Computers** connected via Switch for basic connectivity test
- 🌐 **Web Server** hosting a landing page
- 📧 **Email Server** for internal mail simulation
- 📁 **FTP Server** for file exchange
- 🧠 **IoT Sensors** and an **IoT Server**
- 🏠 **Home Devices** (like Smart Thermostat) securely communicating with office devices
- 📦 **VLANs** to isolate Home, Office, IoT zones
- 📡 **Router-on-a-Stick** setup for inter-VLAN routing
- 🔐 **ACLs** to restrict unauthorized access

---

## 🧠 How Home & Office Devices Communicate

> ❓**Why are Home Devices talking to Office Devices?**

Although VLANs isolate traffic, **Inter-VLAN Routing** is enabled to allow **selective, secured communication**, such as:

| From             | To                  | Status        | Reason                                           |
|------------------|---------------------|---------------|--------------------------------------------------|
| Office PC        | Home IoT Device     | ✅ Allowed     | For monitoring IoT sensors                       |
| Home Laptop      | Office Web Server   | ❌ Blocked     | Enforced via ACLs                                |
| Office PC        | FTP/Email Server    | ✅ Allowed     | Internal usage for services                      |
| IoT Sensor       | IoT Server          | ✅ Allowed     | Sensor → Data → Server flow                      |
| Home Devices     | Office PC           | ❌ Blocked     | Maintains segmentation and privacy               |

🔐 ACLs are implemented to ensure **only authorized** traffic flows between VLANs. Think of it as a **custom firewall** inside the router.

---

## 🧪 Lab Features and Scenarios

| Feature                 | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| ✅ Basic PC-to-PC Ping  | Confirm end-to-end connectivity via `ping`                                  |
| 🌐 Web Access          | Access welcome page hosted on internal web server                           |
| 📧 Email Exchange      | Use SMTP/POP3 for mail testing                                               |
| 📁 FTP Transfers       | Securely download/upload files inside office VLAN                           |
| 📡 IoT Sensor Traffic  | Simulate sensor readings to a central IoT Server                            |
| 🔐 ACLs                | Ensure role-based and zone-based access control                             |
| 🧑‍💻 CLI Skills         | Practice `show ip route`, `ipconfig`, `show interfaces`, `tracert` and more |

---

## 🧵 Commands You Can Try

```bash
# On Router
show ip route
show ip interface brief
show access-lists

# On PC
ipconfig /all
ping 192.168.x.x
tracert web.local
````

---

## 📂 Project Insights

* 🏗️ VLAN Design:

  * VLAN 10 – Office
  * VLAN 20 – IoT
  * VLAN 30 – Home
* 🎛️ Inter-VLAN Routing: Router-on-a-stick (Sub-interfaces on Fa0/0.10, Fa0/0.20, etc.)
* 🔑 DHCP used in each VLAN
* 🧱 ACLs: Inbound/outbound filters on sub-interfaces to block/allow by IP or port

---

## 📫 Author

**👤 Saad Khan**
📧 Email: [saado652004@gmail.com](mailto:saado652004@gmail.com)
🐙 GitHub: [@saadoxyz](https://github.com/saadoxyz)

---

## 💡 Tip for Presenting

> *“We designed this Cisco PT network to reflect real-world segmentation using VLANs. We allowed controlled access between home and office zones via inter-VLAN routing, and protected each zone using ACLs. The result is a flexible, secure smart network simulation.”*

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer&customColorList=11,17,25" />
</div>
```
