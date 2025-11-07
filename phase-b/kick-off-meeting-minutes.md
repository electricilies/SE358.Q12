# Kick-off Meeting Minutes

|     |     |
| --- | --- |
| # **KICK-OFF**<br><br># **MEETING MINUTES** | Number: 01 |
| Issued Date: 01/09/2025 |
| Page number: |

|     |     |     |     |
| --- | --- | --- | --- |
| Meeting Purpose | Project kick-off meeting |     |     |
| Meeting Location | Google Meet |     |     |
| Meeting Date | 01/09/2025 | Meeting Time | 9:00 AM |
| Facilitator | Trần Nguyễn Thái Bình (PM) |     |     |
| Project Name | Electricilies |     |     |

| ## Representatives |     |     |     |
| --- | --- | --- | --- |
| No. | Name | Role | Note |
| 1   | Trần Nguyễn Thái Bình | PM  |     |
| 2   | Nguyễn Thái Gia Nguyễn | Developer Team |     |
| 3   | Trần Nguyễn Duy Minh | Developer Team |     |
| 4   | Đào Duy Vinh | Developer Team |     |
| 5   | \[Stakeholders\] | Stakeholders |     |

## 1\. Project Introduction

- Electricilies is an e-commerce platform, designed to provide a comprehensive online marketplace to buy and sell electronic products. The system allows customers to browse products, manage their cart and purchase products with preferred payment methods.
- Electricilies also includes a CMS system for Administrators and Staff members to manage the website.

## 2\. Project Objectives

- Aims to provide a user-friendly, responsive e-commerce system by the end of the project timeline (3 months).
- Includes secure payment gateway integration.
- Connects electronic providers to the system, allowing publishers to be updated with the project status monthly.

## 3\. Methodology

- Development will follow the Incremental Model in the span of 3 months.
- Tools:
  - Jira: Task, backlog management
  - Github: version control system
  - Github Actions: CI/CD
  - Figma: UI/UX design

## 4\. Team Roles

- Project Manager: Bình
- Designer: Minh, Vinh
- Front-end Dev Team: Minh, Vinh
- Back-end Dev Team: Binh, Nguyễn
- Testing Team:
  - Unit Testing & Integration Testing:
    - Front-end: Minh, Vinh
    - Back-end: Bình, Nguyễn
  - E2E Testing: Bình, Vinh

## 5\. Stakeholder Questions

- Q: How many products will the system aim to support for display?
  - A: The system will support at least 100 products.
- Q: Will there be a mobile version app in the future?
  - A: If the initial launch of the project proves to be successful, we will take that into consideration.
- Q: Which payment gateways are planned to be integrated?
  - A: So far, we are planning to integrate VNPay Bank transfer & Credit Card.
- Q: What hosting or environment will be used? Are there any risks or downsides while using these?
  - A: We will deploy it on-premises. But it is possible to bring the app to cloud (AWS, GCP, Azure) thanks to Kubernetes deployment.
- Q: How often will the project status be reported to stakeholders?
  - A: Monthly.
- Q: How will user data be protected and encrypted?
  - A: Keycloak - self-hosted identity and access management - will store the user information, so it will be secured. When the user is deleted from the system, the data is persisted for analytics purposes, but there is no link to the user information, which is deleted entirely in Keycloak.
- Q: Will the system be dependent on external suppliers?
  - A: Yes, therefore before the initial launch, we will have contacted and successfully partnered with suppliers beforehand to provide products to the system.