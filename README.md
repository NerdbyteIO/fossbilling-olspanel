<!-- NerdByte Branding -->

<p align="center">

  <img src="assets/NerdByteLabs.png" alt="NerdByte Labs Text Logo" height="150">

</p>

<p align="center">

  <img src="assets/banner.svg" alt="FOSSBilling OLSPanel Server Module Banner">

</p>

<p align="center">

  <img src="https://img.shields.io/badge/Codeberg-Primary%20Repo-2185D0?style=for-the-badge" alt="Codeberg Primary">

  <img src="https://img.shields.io/badge/GitHub-Mirror-24292F?style=for-the-badge" alt="GitHub Mirror">

  <img src="https://img.shields.io/badge/PHP-8.1%2B-8892BF?style=for-the-badge&logo=php&logoColor=white" alt="PHP Version">

  <img src="https://img.shields.io/badge/FOSSBilling-0.5%2B-5A189A?style=for-the-badge" alt="FOSSBilling Compatibility">

  <img src="https://img.shields.io/badge/status-active-5A189A?style=for-the-badge" alt="Status">

</p>

---

# FOSSBilling OLSPanel Server Module

An open source server management module that integrates **OLSPanel** with **FOSSBilling**, enabling automated hosting account provisioning and lifecycle management.

This project is **community-developed and maintained** by NerdByte and is not officially affiliated with OLSPanel or FOSSBilling.

---

## 🌐 Repository & Contributions

The **primary repository is hosted on Codeberg**:

👉 https://codeberg.org/nerdbyteio/fossbilling-olspanel

GitHub is used only as a **mirror**.

- 💬 Issues: Please open all issues on Codeberg
- 🔀 Pull Requests: Submit all PRs on Codeberg
- 📦 Releases: Published via Codeberg

---

## About This Project

The FOSSBilling OLSPanel Server Module provides a clean and maintainable integration between OLSPanel-powered hosting servers and the FOSSBilling automation platform.

It allows hosting providers and developers to provision and manage customer accounts directly from within FOSSBilling while leveraging the performance and flexibility of OLSPanel.

The goal of this project is to provide:

- A lightweight and reliable integration
- Clear, maintainable code structure
- Predictable automation behavior
- Extensibility for future enhancements

---

## Features

- ✅ Provision new users and domains  
- ✅ Suspend accounts  
- ✅ Unsuspend accounts  
- ✅ Change account passwords  
- ✅ Cancel and permanently delete accounts  

Additional improvements and refinements are released incrementally.

---

## Installation

1. Download the `OLSPanel.php` file from this repository.
2. Copy the file to your FOSSBilling installation: `/library/server/manager/OLSPanel.php`
3. Log in to the FOSSBilling Admin Panel.
4. Navigate to **System → Servers**.
5. Create a new server using the **OLSPanel** server manager.
6. Configure authentication and connection details as required.

---

## Requirements

- PHP 8.1 or higher
- FOSSBilling 0.5 or higher
- Active OLSPanel server instance
- Valid OLSPanel administrative credentials

---

## Required Custom Package Configuration

The following custom parameters must be defined for each product in FOSSBilling:

- **pkg_id**  
  The Package ID from OLSPanel.

- **php_version**  
  The PHP version assigned to the package (e.g., `8.1`, `8.2`).

Location in FOSSBilling: `Products → Edit Product → Custom Parameters`

---

## How to Locate the Package ID in OLSPanel

1. Log in to your **OLSPanel Admin Panel**.
2. Navigate to **Users → Package**.
3. Click **Manage** on the desired package.
4. The final number in the URL is the **Package ID**.

Example:  
If the URL ends in `/1/`, then: `pkg_id = 1`

Ensure:
- `yourolspaneldomain` matches your server hostname or IP
- `panelport` matches your configured OLSPanel port

---

## Disclaimer

FOSSBilling OLSPanel Server Module is an independent open source project developed by NerdByte.

It is **not affiliated with, endorsed by, or sponsored by**:

- OLSPanel  
- FOSSBilling  

---

## Support the Project

https://buymeacoffee.com/devjsonio
