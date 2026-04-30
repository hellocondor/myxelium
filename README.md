## Myxelium Converged ISP Cloud Platform

**Myxelium** is a multi-tenant, cloud-native platform that unifies **AAA, OSS and BSS** for Internet Service Providers. It provides a single control plane to manage subscribers, network access, CPEs, billing, and support operations at scale.

---

## Overview

ISPs typically operate fragmented systems for authentication, billing, device provisioning, and customer support. Myxelium consolidates these into a **cohesive, API-driven platform** designed for automation, scalability, and operational clarity.

---

## Core Modules

* **Cloud AAA**
  Centralized authentication, authorization, and accounting for subscriber sessions.
* **Cloud RADIUS**
  High-performance RADIUS service for network access control, policy enforcement, audit and troubleshooting.
* **Cloud ACS (Automatic Configuration Server )**
  Remote provisioning and lifecycle management of CPE devices using CWNP TR-069/TR-369.
* **Cloud DMS (Device Management System)**
  Inventory, monitoring, and configuration management for network devices and ONTs.
* **Cloud Billing**
  Usage-based and subscription billing with invoicing and payment tracking.
* **Cloud Ticketing**
  Customer support workflows, issue tracking, and service resolution.

---

## Core Modules

* **Cloud AAA**
  Centralized authentication, authorization, and accounting for subscriber sessions.
* **Cloud RADIUS**
  High-performance RADIUS service for network access control and policy enforcement.
* **Cloud ACS (TR-069/TR-369)**
  Remote provisioning and lifecycle management of CPE devices.
* **Cloud DMS (Device Management System)**
  Inventory, monitoring, and configuration management for network devices and ONTs.
* **Cloud Billing**
  Usage-based and subscription billing with invoicing and payment tracking.
* **Cloud Ticketing**
  Customer support workflows, issue tracking, and service resolution.

---

## Key Capabilities

* **Multi-Tenant Architecture**
  Isolated environments for multiple ISPs or business units within a single deployment.
* **Unified Subscriber View**
  Single source of truth across AAA sessions, devices, billing, and support.
* **Real-Time Control Plane**
  Instant policy enforcement and session visibility.
* **API-First Design**
  Fully automatable via REST APIs for integration with external systems.
* **Scalable & Cloud-Native**
  Designed for containerized deployment and horizontal scaling.

---

## Architecture

Myxelium follows a modular microservices architecture:

* Stateless services for control and orchestration
* Dedicated services for AAA, RADIUS, ACS, and billing
* Event-driven communication between modules
* Centralized datastore per tenant boundary

---

## Use Cases

* Broadband ISPs (FTTH, Fixed Wireless)
* Multi-tenant network operators
* Managed service providers
* ISP startups requiring rapid deployment

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/hellocondor/myxelium.git

cd myxelium

# Start services
docker-compose up -d
```

Access the platform:

```
http://localhost:3000
```

---

## Tech Stack

* **Backend:** Node.js / Go
* **Frontend:** React
* **Database:** PostgreSQL / Redis
* **Networking:** RADIUS, TR-069/TR-369,
* **Deployment:** Docker, Nginx

---

## Philosophy

Myxelium is built around one principle:

> **Control the subscriber, control the network.**

By converging AAA, device management, and business systems, ISPs gain full visibility and control over service delivery and customer experience.

---

## License

MIT License

---

## Status

Active development — not production-ready.
