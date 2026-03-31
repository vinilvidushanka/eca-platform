# ITS 2130 ECA Project Submission - Platform Layer

Polyrepo architecture with Git submodules, implemented with Spring Cloud and deployed on Google Cloud Platform.

## 1. Student Information

| Field | Value |
| :--- | :--- |
| **Module** | ITS 2130 Enterprise Cloud Application |
| **Program** | HDSE @ IJSE |
| **Student Name** | Vinil Vidushanka |
| **Student ID** | 2301692013 |
| **Submission Date** | 2026-03-31 |
| **Main Submission Repository** | https://github.com/vinilvidushanka/eca-platform.git |
| **GCP Project ID** | godrive-eca-project |

## 2. Project Overview

This repository contains the core infrastructure and platform services for the **GoDrive** project.
* It follows a polyrepo architecture using Git submodules.
* All platform components are implemented using Spring Cloud.
* The system is fully deployed on Google Cloud Platform (GCP).

## 3. Live Public URLs (Mandatory)

| Component | Public URL |
| :--- | :--- |
| **Eureka Dashboard (Mandatory)** | http://34.93.114.63:8761/ |

## 4. Repository Structure (Polyrepo + Submodules)

### 4.1 Nested Submodules in Platform

| Path | Repository | Purpose |
| :--- | :--- | :--- |
| Platform/api-gateway | https://github.com/vinilvidushanka/API-Gateway-GoDrive.git | API Gateway |
| Platform/config-server | https://github.com/vinilvidushanka/Config-Server-GoDrive.git | Spring Cloud Config Server |
| Platform/eureka-server | https://github.com/vinilvidushanka/Eureka-Server-GoDrive.git | Eureka Service Registry |

## 5. Spring Cloud Components Implemented

* Spring Cloud Config Server
* Spring Cloud Netflix Eureka Server
* Spring Cloud API Gateway

## 6. High Availability and Auto Scaling (Mandatory)

### 6.1 Platform High Availability

| Check | Value |
| :--- | :--- |
| Multi-instance deployment | YES |
| Multi-zone deployment | asia-southeast1-a, asia-southeast1-b, asia-southeast1-c |
| Fault-tolerance evidence | YES |

## 7. PM2 Process Management and Auto Restart (Mandatory)

Applications are managed by PM2 to ensure reliability and process-level fault tolerance as per the module guidelines.

### 7.1 PM2 Compliance Checklist

| Requirement | Status |
| :--- | :--- |
| Applications started and managed by PM2 | YES |
| Logs written to correct location | YES |
| Auto restart on failure | YES |
| PM2 starts on VM reboot | YES |

## 8. How to Clone This Repository

```bash
git clone --recurse-submodules [https://github.com/vinilvidushanka/eca-platform.git](https://github.com/vinilvidushanka/eca-platform.git)
