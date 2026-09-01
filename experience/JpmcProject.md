## Project: Mail Management Service (MMS)

### Project Overview

**Mail Management Service (MMS)** is a backend, event-driven application responsible for managing enterprise Microsoft Exchange mailbox and mail-related operations across different mailbox and messaging entities.

The service provides end-to-end processing of mail management requests, including operations for:

- Individual/User Mailboxes
- Service Account Mailboxes
- Shared Mailboxes
- Distribution Lists

MMS orchestrates mail operations between **Microsoft Exchange Server 2019** and **Active Directory (AD)** to ensure consistency and integrity of mailbox-related information across the underlying enterprise systems.

The application processes requests originating from enterprise service-management workflows and coordinates the required backend operations across multiple services. Once processing is completed, MMS communicates the final operation status back to the requesting service, providing clear success or failure information.

The application follows an **event-driven microservices architecture**, where Kafka is used for asynchronous communication between services. This architecture helps improve application resilience and durability, particularly for operations involving external systems that may experience temporary availability issues or require longer processing times.

---

## Responsibilities

Worked as a **Spring Boot Backend Developer** responsible for developing, enhancing, securing, deploying, and supporting the Mail Management Service.

Key responsibilities included:

- Developed and enhanced backend features for the Mail Management Service using **Java and Spring Boot**.
- Implemented business functionality across multiple microservices involved in mail management operations.
- Contributed to the end-to-end development and deployment lifecycle of the application.
- Enhanced application security by integrating JPMorgan Chase enterprise security frameworks, tools, and dependencies.
- Improved application **resilience, reliability, and durability** when interacting with external enterprise systems.
- Replicated and configured the MMS application for the **China region**, including region-specific application configuration, security, infrastructure, and Active Directory integration.
- Deployed and supported the application across multiple environments and platforms, including **Cloud and VSI environments running Unix and Windows**.
- Investigated and resolved production incidents by performing root-cause analysis, identifying application defects, and implementing permanent fixes.
- Worked on production deployment activities, post-deployment validation, IP configuration, and load-balancing setup.
- Collaborated with application, infrastructure, security, and platform teams to resolve environment, access, connectivity, and deployment issues.
- Implemented JPMorgan Chase engineering technologies and internal platform capabilities to meet enterprise application requirements.

---

### Backend Development

- Developed backend services using **Java and Spring Boot** following microservice-based architecture.
- Implemented REST APIs using **OpenAPI-based API specifications and development practices**.
- Developed and enhanced business functionality required for enterprise mail management operations.
- Integrated backend services with enterprise systems including **Microsoft Exchange Server and Active Directory**.
- Implemented integrations with JPMorgan Chase internal enterprise security systems following **OAuth and token-based security patterns**.
- Designed backend functionality to handle communication with external systems while maintaining reliable request processing and appropriate error handling.
- Implemented configuration-driven functionality to support different deployment environments and regional requirements.

---

### Enterprise Password & Secret Management

- Implemented enterprise password retrieval mechanisms using **Enterprise Password Vault (EPV)** for secure retrieval of application credentials and secrets.
- Configured the application to securely consume credentials required for communication with dependent enterprise systems.
- Contributed to the migration of secret-management functionality from **EPV to GSM** as part of the organization's platform evolution.
- For the China-region deployment, implemented integration with **CyberArk** for secure password and credential retrieval.
- Ensured application and deployment configurations followed enterprise security requirements for handling sensitive credentials.

---

### Kafka & Event-Driven Architecture

Kafka-based event processing is a core part of the MMS architecture.

- Implemented and enhanced asynchronous communication between MMS microservices using **Apache Kafka**.
- Used Kafka messaging to decouple services and reduce dependency on synchronous communication between backend components.
- Leveraged Kafka's message-processing and retry capabilities to improve application resilience when downstream systems or dependent services experience temporary failures.
- Designed message-driven processing to support operations that may require longer execution times due to external server or database dependencies.
- Contributed to reliable request processing by ensuring messages could be reprocessed when transient failures occurred.
- Worked with Kafka-based workflows to improve the overall **durability, fault tolerance, and reliability** of the application.

---

### Active Directory Integration

- Developed a reusable REST API service for performing **Active Directory operations**.
- Implemented AD operations using **Spring LDAP / LdapTemplate** and LDAP queries.
- Designed the API to be consumed by multiple MMS services and other application teams.
- Implemented LDAP-based communication for enterprise directory operations.
- Enhanced LDAP authentication and configuration to support application requirements.
- Contributed to configuring and validating **China-region Active Directory integration**.
- Troubleshot connectivity, configuration, authentication, and environment-specific issues while integrating application services with Active Directory.
- Ensured AD-related operations were handled consistently with the corresponding mail-management workflows.

---

### Security & Authentication

- Implemented end-to-end application security for the **China-region MMS deployment** using JPMorgan Chase enterprise security frameworks, dependencies, and approved security mechanisms.
- Integrated JPMorgan Chase internal security tooling for authentication and authorization across application components and deployment environments.
- Implemented **OAuth/token-based authentication** for secured REST API communication.
- Configured application security components across different deployment environments.
- Implemented secure credential retrieval using **CyberArk** for the China environment.
- Investigated and resolved security and connectivity issues caused by differences between application requirements and **VSI-compatible network and security configurations**.
- Worked with infrastructure and security teams to resolve certificate, network, access, and authentication-related deployment issues.
- Ensured security configurations were consistently applied across application runtime and deployment environments.

---

### CI/CD & Production Support

Worked extensively with the organization's internal CI/CD ecosystem to automate and manage application deployments.

#### Jules

- Developed and configured **Jules deployment files** for the China-region MMS application.
- Worked with deployment configurations involving **AIM variables, GAP variables, AIM artifacts, and Cloud Foundry (CF) commands**.
- Built the deployment configuration required to support the end-to-end China application deployment workflow.
- Troubleshot and resolved multiple deployment issues related to access, permissions, configuration, environment setup, and platform dependencies.

#### AIM — Application Infrastructure Manager

- Worked with **AIM (Application Infrastructure Manager)** as part of the application's CI/CD process.
- Used AIM artifacts and configuration to support secure artifact delivery during deployments.
- Worked with AIM-related authentication and authorization requirements for the continuous delivery workflow.

#### GAP — Gaia Application Platform

- Worked with **GAP (Gaia Application Platform)** as the application hosting and deployment platform.
- Configured application deployment requirements for GAP environments and application instances/pools.
- Troubleshot GAP-related deployment and environment issues.

#### CF — Cloud Foundry

- Worked with **Cloud Foundry (CF)** commands as part of the application deployment and platform-management workflow.
- Used CF commands to execute deployment-related operations and manage application services within the cloud environment.
- Investigated and resolved deployment failures involving application configuration, permissions, connectivity, and platform dependencies.

---

### Deployment & Infrastructure

- Deployed the MMS application across multiple environments, including **Cloud and VSI platforms**.
- Supported deployments across both **Unix and Windows-based VSI environments**.
- Performed post-production deployment activities including IP configuration and application connectivity validation.
- Worked on **load-balancer configuration** to support application traffic distribution and availability.
- Troubleshot infrastructure-related issues affecting application availability and connectivity.
- Collaborated with infrastructure teams to resolve environment-specific deployment and network issues.
- Supported application configuration and infrastructure setup for the China-region MMS deployment.

---

### Production Support & Incident Management

- Acted as a primary support resource for resolving application incidents raised by clients and users.
- Analyzed production issues using application logs, error information, and system behavior.
- Performed **Root Cause Analysis (RCA)** to identify the underlying cause of production defects.
- Implemented and deployed fixes for identified application defects.
- Supported post-fix validation to ensure incidents were permanently resolved.
- Collaborated with dependent application and infrastructure teams when incidents involved external systems.
- Participated in production troubleshooting and application stability improvements.

---

### Testing & Quality Assurance

- Performed manual **Sanity Testing** following application deployments and configuration changes.
- Executed manual **Regression Testing** to verify that new changes did not impact existing functionality.
- Performed functional validation of backend services and API behavior.
- Conducted post-deployment validation across different environments.
- Supported defect identification and verification of fixes before production release.

---

## Technology Stack

| Category | Technologies / Tools |
|---|---|
| Programming Language | Java |
| Framework | Spring Boot |
| Architecture | Microservices, Event-Driven Architecture |
| API | REST APIs, OpenAPI |
| Messaging | Apache Kafka |
| Directory Services | Active Directory, LDAP, Spring LdapTemplate |
| Mail Platform | Microsoft Exchange Server 2019 |
| Security | OAuth, Token-Based Authentication, JPMorgan Chase Internal Security Frameworks |
| Secret Management | EPV, GSM, CyberArk |
| Cloud Platform | GAP — Gaia Application Platform |
| Deployment | Cloud Foundry (CF), Jules |
| Infrastructure | AIM — Application Infrastructure Manager, Load Balancers |
| Environments | Cloud, VSI — Unix & Windows |
| Testing | Manual Sanity Testing, Regression Testing |
| Support | Production Support, Incident Management, Root Cause Analysis |

---

## Key Contributions

- Contributed to the development and enhancement of a **mission-critical enterprise Mail Management Service**.
- Improved application **resilience and durability** through asynchronous Kafka-based processing and reliable message handling.
- Developed reusable **Active Directory REST APIs** consumed by multiple services and teams.
- Implemented end-to-end security and secret-management integration for the **China-region MMS deployment**.
- Successfully replicated and configured MMS for the China environment across application, security, AD, infrastructure, and deployment layers.
- Built the **China-region Jules CI/CD deployment configuration** and resolved complex access, permission, configuration, and platform-related issues.
- Supported application deployment across **Cloud and VSI environments**, including Unix and Windows platforms.
- Contributed to infrastructure activities including **load-balancer and post-deployment network configuration**.
- Resolved production incidents through systematic troubleshooting, root-cause analysis, and permanent defect fixes.
- Contributed to the adoption and implementation of **JPMorgan Chase enterprise engineering and innovative technologies**.