
Azure & Microsoft 365 Infrastructure Setup

Overview

This project provides a step-by-step PowerShell script to set up a secure cloud infrastructure using Microsoft 365 and Azure services. The script is organized into phases, enabling IT administrators to configure Azure AD, enforce security policies, deploy endpoint protection, and set up backup solutions incrementally.

Each phase is modular, allowing customization based on specific needs. This repository is ideal for organizations seeking a scalable, secure, and compliant Microsoft 365 and Azure environment.

Table of Contents

	•	Prerequisites
	•	Phases Overview
	•	Phase 1: Azure AD and Microsoft 365 Setup
	•	Phase 2: Microsoft 365 Security Configurations
	•	Phase 3: Endpoint Security with Defender for Endpoint
	•	Phase 4: Backup Configuration with Azure Recovery Services
	•	Phase 5: Documentation and Automation
	•	How to Use
	•	Contribution Guidelines
	•	License

Prerequisites

	1.	PowerShell: Ensure you’re running PowerShell 5.1 or later.
	2.	Modules:
	•	AzureAD Module for Azure AD management.
	•	ExchangeOnlineManagement Module for Exchange Online configuration.
	•	Defender Module for Defender security settings.
	•	Azure PowerShell Module for Azure resource management.
	3.	Permissions: Ensure you have administrator privileges in both Microsoft 365 and Azure to perform these configurations.

Phases Overview

Phase 1: Azure AD and Microsoft 365 Setup

This phase initializes Azure AD and creates foundational user groups and accounts. It includes:

	•	Connecting to Azure AD
	•	Creating user groups for different departments (e.g., Finance, Legal)
	•	Adding users and assigning them to appropriate groups

Script for Phase 1

Phase 2: Microsoft 365 Security Configurations

In this phase, we configure essential Microsoft 365 security policies, including:

	•	Enabling Multi-Factor Authentication (MFA) for all users
	•	Setting up a Data Loss Prevention (DLP) policy to protect sensitive information
	•	Enabling a Conditional Access policy to block legacy authentication

Script for Phase 2

Phase 3: Endpoint Security with Defender for Endpoint

This phase configures Microsoft Defender for Endpoint to protect against potential threats. Key configurations include:

	•	Enabling PUA protection and Controlled Folder Access
	•	Configuring trusted applications for Controlled Folder Access
	•	Setting up periodic scans

Script for Phase 3

Phase 4: Backup Configuration with Azure Recovery Services

In this phase, we configure backup solutions using Azure Recovery Services for data protection. It includes:

	•	Creating a Recovery Services Vault in Azure
	•	Registering and protecting VMs with automated backup policies
	•	Setting up backup monitoring for data integrity

Script for Phase 4

Phase 5: Documentation and Automation

The final phase automates the documentation of configuration settings and schedules regular backups. It includes:

	•	Exporting user and group data for documentation
	•	Scheduling automated backups via PowerShell and Task Scheduler or Azure Automation

Script for Phase 5

How to Use

	1.	Clone the Repository: Download this repository to your local machine.

git clone https://github.com/YourUsername/Azure-M365-Infrastructure-Setup.git


	2.	Run Each Phase:
	•	Open PowerShell with administrator privileges.
	•	Navigate to the folder containing the scripts for each phase.
	•	Run each phase script in sequence, modifying parameters (like usernames and group names) as needed.
	3.	Secure Sensitive Data: Ensure all passwords and credentials are stored securely and not hard-coded into the scripts.
	4.	Schedule Regular Backups (Phase 5): Use Task Scheduler or Azure Automation to schedule the backup script for regular intervals.

Contribution Guidelines

Contributions to improve this repository are welcome! If you have suggestions or updates, please follow these steps:

	1.	Fork the repository.
	2.	Create a new branch for your feature.
	3.	Submit a pull request with a detailed description of the changes.

Please ensure that your contributions follow best practices and are tested before submitting.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Disclaimer

This script is provided as-is. Ensure compliance with your organization’s security policies and requirements before deploying to a production environment. Always test configurations in a safe, non-production environment when possible.

This README file provides a comprehensive guide for users to understand and use the PowerShell scripts, ensuring the setup process is clear and documented for both deployment and future reference.
