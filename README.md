# 🏠 Homelab

This is my personal homelab that I’ve been building out to get more hands-on experience with infrastructure, networking, and virtualization. One of the questions I was asked at my current role is how do I keep up with technology constantly evolving?  Have I built a homelab?  I felt lucky to still be offered a role when I flat out did not have any homelab to show.  I don't want to leave that up to luck again, so I went ahead and ordered several pieces of gear and tech to finally get myself my very own homelab!

---

## What I’m Running

- **Switch:** Ubiquiti Switch Lite 8  
- **Access Point:** Ubiquiti WiFi 7 Lite  
- **DNS / Ad Blocking:** Raspberry Pi 5 running Pi-hole  
- **Compute:** 2x Lenovo hosts running Proxmox (clustered)

---

## Setup Overview

### Proxmox Cluster
I’m running two Lenovo machines in a Proxmox cluster so I can manage everything from a single dashboard. This lets me spin up VMs/containers easily and treat both hosts as one environment instead of juggling them separately.

### Network
Everything runs through Ubiquiti gear. It’s simple, reliable, and gives me room to grow the network over time if I want to start segmenting things or adding more devices.

### Pi-hole
The Raspberry Pi 5 is running Pi-hole as my network-wide DNS sinkhole. It handles ad blocking and gives me more visibility into traffic across my network.

### Virtualization / Lab Use
The Proxmox hosts are where I experiment with different services, containers, and ideas. This is basically my sandbox for anything infrastructure-related—whether that’s testing tools, breaking things, or rebuilding them better.

---

## 🔧 Tech I’m Using

- Proxmox VE  
- Pi-hole & Raspberry Pi 5
- Ubiquiti (UniFi)  
- Linux (across hosts and VMs)  

---

## Why I Built This

- The main reason was to provide improved internet across my house.  While I have fiber internet and it works wonderfully with a wired connection, the wifi was lacking.  I decided to add an additional Wifi Access Point on my second floor on an opposite side of my house as my router.  While I was at it, I converted all of the old phone landlines in my house into RJ45 enabled ports, that way I can connect direction to my Ubiquiti Switch on any floor of my house.
- While I was at it, I figured it would make sense to get more comfortable with building Linux hosts from scratch!  I am running Pi-hole on a Raspberry Pi 5 that acts as the primary DNS.  I also have two Lenovo Workstations that both are running Proxmox.  They are on the same Proxmox Cluster, that way I can configure both on the same dashboard and allow them to utilize a shared drive for similar needs such as ISO files.
- Learn more about virtualization, clustering, and system management
- Practice networking concepts in a real environment  
- Have a place to experiment with DevOps / cloud-related tools while also self hosting my own applications that I want to build 

---

## What I Want to Add Next

- Monitoring (Prometheus / Grafana)
- Automated backups for VMs and containers
- VLANs + better network segmentation
- Possibly expanding the cluster with more nodes or storage
- Self hosted websites
- Possibly home automation
