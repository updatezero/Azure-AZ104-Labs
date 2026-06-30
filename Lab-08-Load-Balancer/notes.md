# Notes - Lab 08

## What I learned

This lab introduced Azure Load Balancer and its purpose in providing high availability and traffic distribution across multiple backend resources.

Unlike assigning a Public IP directly to a Virtual Machine, Azure Load Balancer sits in front of one or multiple backend servers and distributes incoming traffic according to configured rules.

---

## Azure Load Balancer

Azure Load Balancer is a Layer 4 (Transport Layer) Load Balancer.

It distributes traffic based on:

- Source IP
- Destination IP
- Source Port
- Destination Port
- Protocol (TCP / UDP)

---

## Types

### Public Load Balancer

- Internet facing
- Uses a Public IP
- Receives external traffic

### Internal Load Balancer

- Private IP only
- Used inside Azure Virtual Networks
- Internal applications

---

## SKU

### Standard

Recommended.

Advantages:

- Higher availability
- Better security
- Zone redundancy
- Production workloads

---

## Frontend IP

The Frontend IP is the address clients connect to.

A Load Balancer requires its own Public IP.

A Public IP already attached to a Virtual Machine cannot simultaneously be attached to a Load Balancer.

During this lab I created a dedicated Public IP specifically for the Load Balancer.

---

## Backend Pool

The Backend Pool contains the resources receiving traffic.

Examples:

- Virtual Machines
- Virtual Machine Scale Sets

Traffic is distributed between backend members.

---

## Health Probes

Health probes continuously check whether backend servers are healthy.

If a VM stops responding:

- Azure removes it from the Load Balancer
- Traffic is automatically redirected to healthy servers

This increases availability.

---

## Inbound Rules

Inbound Rules define:

- Frontend Port
- Backend Port
- Protocol
- Backend Pool

Example:

80 → HTTP

443 → HTTPS

3389 → RDP

---

## Outbound Rules

Outbound Rules allow backend servers to initiate outbound Internet connections through the Load Balancer.

---

## Public IP

Every Public Load Balancer requires a Public IP resource.

Best practice is to assign a dedicated Public IP instead of reusing the VM's existing Public IP.

---

## High Availability

A Load Balancer helps eliminate single points of failure.

If multiple backend servers exist:

- Traffic is balanced
- Failed servers stop receiving traffic
- Healthy servers continue serving requests

---

## AZ-104 Knowledge

After completing this lab I understand:

- Azure Load Balancer architecture
- Layer 4 Load Balancing
- Frontend IP configuration
- Backend Pools
- Public vs Internal Load Balancers
- Standard SKU
- Health Probes
- Inbound Rules
- Outbound Rules
- Public IP requirements
- High Availability concepts
- Azure deployment workflow
