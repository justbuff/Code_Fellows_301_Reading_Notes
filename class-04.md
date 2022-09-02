# What is Group Policy (GPO)?

Group Policy (GP) is a feature of Windows that provides a centralized place in the Active Directory (AD) for administrators to manage and configure operating systems, applications and users’ settings. 

A Group Policy Object (GPO) is a group of settings that are created using the Microsoft Management Console (MMC) Group Policy Editor. GPOs can be associated with a single or numerous Active Directory containers, including sites, domains, or organizational units (OUs). The MMC allows users to create GPOs that define registry-based policies, security options, software installation and more.

AD applies GPOs in the same order: local policies, site policies, domain policies and OU policies.

The order that GPOs are processed is known as LSDOU, which stands for local, site, domain, organizational unit. The local computer policy is the first to be processed, followed by the site level to domain AD policies, then finally into organization units. 

GPs can be used in numerous ways to bolster security, including disabling outdated protocols, preventing users from making certain changes and more.

Other GP advantages:

- Password Policy: GPOs can be used to establish password length, complexity and other requirements.

- Systems Management: GPOs can be used to simplify tasks

- Health Checking: GPOs can be used to deploy software updates and system patches

GPO Limitations:

- GPO editor isn’t the most user-friendly console

- GPO updates are undertaken randomly every 90 to 120 minutes or whenever the computer gets rebooted

- GPOs are not immune to cyberattacks
