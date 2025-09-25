# Web Infrastructure Design

## 🧠 Project Overview

This project focuses on designing scalable and robust web infrastructures. You will conceptualize and illustrate realistic web architectures to support high-traffic websites, addressing concerns such as load balancing, redundancy, scalability, and monitoring. The emphasis is on understanding how components interact across layers—from DNS resolution to database replication—while optimizing for fault tolerance and performance.

## 🎯 Learning Objectives

By completing this project, you will learn to:

- Design scalable and highly available web infrastructures.
- Explain how DNS, firewalls, load balancers, and web servers interact.
- Model replication between database servers (MySQL primary/replica).
- Integrate monitoring and understand system limitations.
- Create detailed architecture diagrams using tools like `draw.io`.

---

## 📌 Tasks

### Task 0: Simple Web Stack

**Objective**: Design a basic web infrastructure.

**Requirements**:
- 1 client accesses `www.foobar.com`
- DNS resolves to the Load Balancer IP
- Load balancer forwards traffic to a single web server
- Web server is connected to a single MySQL database
- The database and web server share application files

**Expected Outcome**:
A simple, linear design showing DNS → Load Balancer → Web Server → MySQL.

---

### Task 1: Distributed Web Infrastructure

**Objective**: Add redundancy to the web infrastructure.

**Requirements**:
- Multiple web servers
- Load balancing across web servers
- Redundant database servers (with one set as replica)
- Each web server connects to the primary DB

**Expected Outcome**:
A fault-tolerant design with multiple web servers and a replicated database setup.

---

### Task 2: Secured and Monitored Infrastructure

**Objective**: Add firewalls, HTTPS, and monitoring.

**Requirements**:
- Firewalls between components (client–LB, LB–web, web–DB)
- SSL certificate on Load Balancer (HTTPS traffic)
- Monitoring agents on all servers

**Expected Outcome**:
A production-ready design with basic security and health monitoring.

---

### Task 3: Scale Up

**Objective**: Horizontal scaling of backend services.

**Requirements**:
- Add a third web server (Server C)
- Maintain load balancing (HAProxy cluster)
- Add a third MySQL replica
- Reflect all arrows including HTTPS responses

**Expected Outcome**:
A highly scalable and redundant system with multiple app/db servers and detailed data flows.

---

## 🛠 Tools

- [Draw.io](https://draw.io) or diagrams.net for network schematics
- Markdown for documentation
- `PNG` exports of each design for visual presentation

---

## 🧩 Notes

- All components must be explicitly represented (e.g., firewalls, DB replicas).
- Arrows must indicate both directions of data flow when needed.
- Realistic IPs and hostnames are encouraged for clarity.
- You can use custom icons or emoji for better visual representation.