# Bills Payment API Test Automation

This repository contains the QA automation suite for the **WayaBank Bills Payment** system. It includes API tests for electricity, cable TV, and educational E-pins to ensure payment reliability on the staging environment.

## 🚀 API Coverage
The following services from the Postman collection are covered in this suite:

* **Electricity Services**: Fetching providers and purchasing tokens (e.g., Eko Electric).
* **E-Pin Services**: Bulk or single purchase of educational pins like WAEC.
* **Cable TV**: Fetching available cable providers.
* **Validation**: Real-time validation of account and meter numbers.

---

## 🛠 Prerequisites

* [Node.js](https://nodejs.org/) installed on your machine.
* [Newman](https://www.npmjs.com/package/newman) (The CLI tool for running Postman collections).
* Access to the **Staging Environment** for `wayabank.ng`.

---

## ⚙️ Configuration & Security

The collection uses **Bearer Token Authentication**. 

> [!IMPORTANT]
> The current collection contains hardcoded staging tokens. For security, it is recommended to use environment variables (`{{token}}`) and GitHub Secrets when running in a CI/CD pipeline.

### Key Data Points
* **Base URL (v3)**: `https://servicesv3.staging.wayabank.ng`
* **Base URL (General)**: `https://services.staging.wayabank.ng`

---

## 🏃 Execution Guide

### 1. Install Newman
```bash
npm install -g newman
