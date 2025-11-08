# Phase B Report

Class: SE358.Q12
Lecturer: Lê Văn Tuấn

Members:
Nguyễn Thái Gia Nguyễn - 23521049
Đào Duy Vinh - 23521787
Trần Nguyễn Duy Minh - 23520956
Trần Nguyễn Thái Bình - 23520161

# 1. Budget Management

| Component/Task                        | Detailed Item                             | Quantity            | Unit Cost    | Total Cost  |
| ------------------------------------- | ----------------------------------------- | ------------------- | ------------ | ----------- |
| **Personnel Costs**                   |                                           |                     |              |             |
| Business Analyst                      | Monthly salary                            | 1 person × 4 months | $800/month   | $3,200      |
| Software Developer                    | Monthly salary                            | 4 people × 4 months | $1,000/month | $16,000     |
| QA Tester                             | Monthly salary                            | 2 people × 4 months | $700/month   | $5,600      |
| UI/UX Designer                        | Monthly salary                            | 2 people × 4 months | $750/month   | $6,000      |
| Project Manager                       | Monthly salary                            | 2 people × 4 months | $1,200/month | $9,600      |
| DevOps Engineer                       | Monthly salary                            | 1 person × 4 months | $1,100/month | $4,400      |
| **Infrastructure - Hardware**         |                                           |                     |              |             |
| Kubernetes Master Node                | Mini PC (16GB RAM, 256GB NVMe)            | 1 unit              | $250         | $250        |
| Network Switch                        | 8-port Gigabit managed switch             | 1 unit              | $45          | $45         |
| UPS Battery Backup                    | 1000VA UPS for server protection          | 1 unit              | $80          | $80         |
| Network Cables                        | Cat6 Ethernet cables (10ft)               | 5 cables            | $8           | $40         |
| Server Rack/Cabinet                   | Small 6U wall-mount rack                  | 1 unit              | $60          | $60         |
| **Infrastructure - Storage**          |                                           |                     |              |             |
| Backup Storage                        | 500GB External HDD for backups            | 1 unit              | $10          | $10         |
| **Infrastructure - Network & Domain** |                                           |                     |              |             |
| Domain Registration                   | .id.vn domain (1 year)                    | 1 domain            | $3           | $3          |
| SSL Certificate                       | Let's Encrypt (Free)                      | 1 certificate       | $0           | $0          |
| Static IP Address                     | Dedicated static IP (if needed)           | 4 months            | $10/month    | $40         |
| Internet Connection                   | Business internet (100Mbps)               | 4 months            | $60/month    | $240        |
| **Infrastructure - Utilities**        |                                           |                     |              |             |
| Electricity                           | Server power consumption (~300W 24/7)     | 4 months            | $35/month    | $140        |
| Office Space                          | School, Work from home                    |                     | $0           | $0          |
| **Software & Services**               |                                           |                     |              |             |
| Container Registry                    | Github container registry (GHCR)          |                     | $0           | $0          |
| Monitoring Service                    | Self-hosted Prometheus + Grafana          |                     | $0           | $0          |
| Log Management                        | Self-hosted Grafana Loki                  |                     | $0           | $0          |
| Database                              | PostgreSQL (self-hosted)                  |                     | $0           | $0          |
| Cache System                          | Redis (self-hosted)                       |                     | $0           | $0          |
| Identity and Access Management        | Keycloak (self-hosted)                    |                     | $0           | $0          |
| CI/CD Pipeline                        | GitHub Actions (free tier)                |                     | $0           | $0          |
| Message Queue                         | RabbitMQ/Kafka (self-hosted, if needed)   |                     | $0           | $0          |
| Reverse Proxy/Ingress                 | Traefik/Nginx Ingress Controller          |                     | $0           | $0          |
| **Development Tools & Licenses**      |                                           |                     |              |             |
| IDE Licenses                          | VSCode, Neovim                            |                     | $0           | $0          |
| Design Software                       | Figma (Free tier)                         |                     | $0           | $0          |
| API Testing Tool                      | Postman (Free tier), Bruno                |                     | $0           | $0          |
| Project Management                    | Jira Software Free                        |                     | $0           | $0          |
| Documentation                         | VitePress with Github Pages               |                     | $0           | $0          |
| Communication                         | Facebook Messenger, Telegram              |                     | $0           | $0          |
| Version Control                       | Git, GitHub (Free)                        |                     | $0           | $0          |
| Database Management                   | DBeaver Community                         |                     | $0           | $0          |
| **Testing & QA**                      |                                           |                     |              |             |
| Load Testing Tool                     | Grafana K6 (open-source)                  |                     | $0           | $0          |
| Browser Testing                       | Playwright with CI                        |                     | $0           | $0          |
| Test Coverage                         | Codecov (Free for open source)            |                     | $0           | $0          |
| Security Scanning                     | SonarQube Community/Cloud (Free tier)     |                     | $0           | $0          |
| API Documentation                     | Swagger/OpenAPI (self-hosted)             |                     | $0           | $0          |
| **Documentation & Assets**            |                                           |                     |              |             |
| Diagram Tools                         | PlantUML                                  |                     | $0           | $0          |
| Image Optimization                    | TinyPNG, ImageOptim (Free tools)          |                     | $0           | $0          |
| **Training & Learning**               |                                           |                     |              |             |
| Online Courses                        | YouTube, freeCodeCamp, MDN                |                     | $0           | $0          |
| Technical Documentation               | Official docs (PostgreSQL, K8s, etc.)     |                     | $0           | $0          |
| **Marketing & Launch**                |                                           |                     |              |             |
| Landing Page Hosting                  | Github Pages (Static site)                |                     | $0           | $0          |
| Email Service                         | Self-hosted or Gmail SMTP                 |                     | $0           | $0          |
| SEO Tools                             | Google Search Console (Free)              |                     | $0           | $0          |
| **Legal & Compliance**                |                                           |                     |              |             |
| Business Registration                 | Company registration fees (if applicable) | 1 time              | $10          | $10         |
| Terms & Privacy Policy                | Legal document templates (online)         |                     | $0           | $0          |
| GDPR Compliance Tools                 | Cookie consent banner (free libraries)    |                     | $0           | $0          |
| **Contingency & Miscellaneous**       |                                           |                     |              |             |
| Hardware Replacement                  | Reserve for hardware failure              | Buffer              |              | $300        |
| Software Emergency                    | Unexpected paid service needs             | Buffer              |              | $150        |
| Team Building                         | Team activities/meals (pizza parties)     | 4 events            | $50          | $200        |
| Office Supplies                       | Whiteboards, markers, notepads, etc.      | Miscellaneous       |              | $100        |
| Emergency Fund                        | General contingency (~5% of operational)  |                     |              | $100        |
| **Subtotal (Operational Costs)**      |                                           |                     |              | **$1,768**  |
| **Subtotal (Personnel Costs)**        |                                           |                     |              | **$44,800** |
| **Grand Total**                       |                                           |                     |              | **$46,568** |

# 2. Quality Plan

## 2.1. Quality Metrics

| **Metric**                         | **Description**                                                                                          | **Measurement Method**                                                           | **Target Value**                          |
| ---------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | ----------------------------------------- |
| **Response Time**                  | Measures how quickly the website loads or responds to user requests.                                     | Performance testing using Playwright.                                            | ≤ 2 seconds per page                      |
| **Defect Density**                 | Number of defects identified during testing per unit size (e.g., per 1,000 lines of code or per module). | (Total number of confirmed defects) ÷ (Size of the software in KLOC or modules). | ≤ 2 defects per KLOC                      |
| **Test Coverage**                  | Percentage of code or features covered by automated or manual tests.                                     | Automatic testing framework (JUnit)                                              | ≥ 80%                                     |
| **Pass Rate**                      | Percentage of executed test cases that passed successfully.                                              | (Number of test cases passed ÷ Total test cases executed) × 100.                 | ≥ 95%                                     |
| **Availability / Uptime**          | Percentage of time the website is operational and accessible to users.                                   | Use uptime monitoring tools (Prometheus/Grafana).                                | ≥ 99.8%                                   |
| **Error Rate**                     | Measures how many API calls or page requests result in errors (e.g., 4xx, 5xx).                          | Analyze server logs and API monitoring dashboards.                               | ≤ 1% of total requests                    |
| **Security Vulnerabilities Found** | Tracks number of security issues identified during testing or audits.                                    | Regular vulnerability scans, penetration testing reports.                        | 0 critical vulnerabilities before release |
| **User Satisfaction**              | Measures how satisfied users are with usability, design, and performance.                                | Post-release surveys, user feedback forms, Net Promoter Score (NPS).             | ≥ 4.2 / 5 average rating                  |

## 2.2. Quality Checklist

| **Quality Task**                                                                  | **Expected Outcome**                                                | **Status** |
| --------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ---------- |
| 1. Conduct performance testing using Playwright for all key pages                 | Each page loads within ≤ 2 seconds under normal conditions          | ☐          |
| 2. Measure and record defect density after system testing                         | Defect density is ≤ 2 defects per KLOC or module                    | ☐          |
| 3. Review automated and manual test coverage reports (JUnit + manual cases)       | Achieve ≥ 80% test coverage across all modules                      | ☐          |
| 4. Execute all planned test cases and log results                                 | ≥ 95% pass rate for all executed tests                              | ☐          |
| 5. Set up uptime monitoring using Prometheus/Grafana                              | Maintain system uptime ≥ 99.8%                                      | ☐          |
| 6. Review error logs and API monitoring dashboard daily                           | Error rate ≤ 1% of total requests                                   | ☐          |
| 7. Perform vulnerability scanning and penetration testing before release          | 0 critical vulnerabilities remaining                                | ☐          |
| 8. Conduct post-release user satisfaction survey (NPS or feedback form)           | Average user rating ≥ 4.2 / 5                                       | ☐          |
| 9. Verify cross-browser compatibility (Chrome, Edge, Firefox, Safari)             | No critical UI or functionality issues on major browsers            | ☐          |
| 10. Review responsive design on multiple devices (desktop, tablet, mobile)        | Layout and performance consistent across devices                    | ☐          |
| 11. Confirm all APIs have proper error handling and status codes                  | All endpoints return correct responses and handle errors gracefully | ☐          |
| 12. Revalidate data integrity after deployment (e.g., orders, products, payments) | No data loss or corruption during transactions                      | ☐          |
| 13. Conduct accessibility audit (WCAG compliance check)                           | Meets minimum WCAG 2.1 AA standards                                 | ☐          |

# 3. Risk Register

| ID  | Date raised | Description                                                                       | Likelihood | Impact | Severity | Owner                               | Mitigation action                                                                                                                                                                            |
| --- | ----------- | --------------------------------------------------------------------------------- | ---------- | ------ | -------- | ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   |             | Staging and production environments not identical, leading to undetectable issues | Medium     | High   | High     | QA Lead, DevOps Engineer            | Implement infrastructure-as-code (IaC) using Kubernetes manifests to ensure environment parity. Conduct regular environment audits and maintain configuration documentation.                 |
| 2   |             | Hardware failure of self-hosted Kubernetes nodes causing service downtime         | Medium     | High   | High     | DevOps Engineer                     | Implement regular backup schedules, maintain UPS power backup, set up monitoring alerts for hardware health. Keep spare hardware components available.                                       |
| 3   |             | Security vulnerabilities in authentication system exposing user data              | Low        | High   | High     | Software Developer, DevOps Engineer | Conduct regular security scans using SonarQube, implement JWT with proper expiration, use HTTPS, apply OWASP best practices, perform penetration testing before launch.                      |
| 4   |             | Database performance degradation with 500+ products and concurrent users          | Medium     | High   | High     | Software Developer, DevOps Engineer | Implement database indexing, query optimization, connection pooling. Use Redis caching for frequently accessed data. Monitor with Prometheus/Grafana.                                        |
| 5   |             | Team member unavailability due to illness or personal issues                      | Medium     | Medium | Medium   | Project Manager                     | Cross-train team members on critical components, maintain comprehensive documentation, establish backup responsibilities for key roles.                                                      |
| 6   |             | Scope creep from stakeholders requesting additional features mid-project          | High       | Medium | Medium   | Project Manager                     | Enforce strict change control process, document all requirements clearly, conduct regular stakeholder meetings to manage expectations.                                                       |
| 7   |             | Internet connection disruption affecting self-hosted services                     | Medium     | High   | High     | DevOps Engineer                     | Implement automatic failover mechanisms, maintain offline development capability, document recovery procedures, consider backup internet connection.                                         |
| 8   |             | Payment gateway (VNPay) integration failures or API changes                       | Low        | High   | High     | Software Developer                  | Implement comprehensive error handling, maintain sandbox testing environment, subscribe to VNPay API change notifications, build abstraction layer for payment processing.                   |
| 9   |             | Insufficient testing coverage leading to bugs in production                       | Medium     | Medium | Medium   | QA Tester                           | Establish minimum 80% code coverage requirement using Codecov, implement automated testing with Playwright and K6, conduct thorough UAT before deployment.                                   |
| 10  |             | Technical debt accumulation from rushed development                               | Medium     | Medium | Medium   | Project Manager, Software Developer | Schedule regular code review sessions, allocate time for refactoring in sprint planning, maintain coding standards documentation, use SonarQube for code quality monitoring.                 |
| 11  |             | Lack of technical expertise in Kubernetes and microservices architecture          | Medium     | High   | High     | DevOps Engineer, Software Developer | Allocate time for team training, leverage online resources (YouTube, official docs), start with simpler deployments and gradually increase complexity, establish knowledge-sharing sessions. |
| 12  |             | Poor performance during load testing (>3 second page load)                        | Medium     | Medium | Medium   | Software Developer, DevOps Engineer | Implement lazy loading, image optimization, CDN for static assets, code splitting. Conduct regular performance testing with K6 throughout development.                                       |
| 13  |             | Data loss due to inadequate backup procedures                                     | Low        | High   | High     | DevOps Engineer                     | Implement automated daily backups to external HDD, test recovery procedures monthly, maintain backup verification logs, consider implementing database replication.                          |
| 14  |             | Communication breakdown among distributed team members                            | Medium     | Medium | Medium   | Project Manager                     | Establish daily stand-ups, use Telegram/Messenger for real-time communication, maintain Jira for task tracking, conduct bi-weekly retrospectives.                                            |
| 15  |             | Budget overrun due to unexpected hardware or service costs                        | Low        | Medium | Medium   | Project Manager                     | Maintain $750 contingency fund, track expenses weekly, prioritize open-source solutions, negotiate with vendors early for any required services.                                             |
| 16  |             | Inadequate documentation causing knowledge gaps                                   | Medium     | Medium | Medium   | All team members                    | Use VitePress for comprehensive documentation, enforce documentation requirements in pull requests, maintain API documentation with Swagger, conduct documentation reviews.                  |
| 17  |             | Keycloak configuration issues causing authentication failures                     | Medium     | High   | High     | DevOps Engineer, Software Developer | Set up dedicated test realm in Keycloak, document all configuration changes, implement monitoring for authentication metrics, maintain rollback procedures.                                  |
| 18  |             | Dependency conflicts or breaking changes in third-party libraries                 | Medium     | Medium | Medium   | Software Developer                  | Use package-lock files, conduct dependency audits regularly, test updates in staging first, maintain changelog for dependency updates.                                                       |
| 19  |             | Compliance issues with GDPR or data protection regulations                        | Low        | High   | High     | Project Manager, Software Developer | Implement cookie consent banners, create Terms & Privacy Policy, ensure data encryption at rest and in transit, conduct compliance review before launch.                                     |
| 20  |             | Missed project deadline of Week 12                                                | Medium     | High   | High     | Project Manager                     | Implement agile methodology with 2-week sprints, track progress weekly using Jira, identify critical path activities, adjust scope if necessary to meet core requirements.                   |

# 4. Human Resource Management

## 4.1. Resource and Personnel Allocation Plan

| Resource Type    | Description                                | Allocation Criteria               | Allocation Plan                                  |
| ---------------- | ------------------------------------------ | --------------------------------- | ------------------------------------------------ |
| Human Resources  | Project team members (business & engineer) | Based on skills and project needs | Assign roles according to expertise and workload |
| Technical Assets | Servers, CI/CD tools, testing frameworks   | Project phase and requirements    | Allocate per development and testing schedule    |
| Time             | Project timeline, milestones               | Project plan and deliverables     | Distribute tasks across sprints and deadlines    |
| Budget           | Funding for tools, infrastructure, support | Project scope and priorities      | Allocate budget for essential resources          |

## 4.2. Roles, Skills, and Workload Identification

| Team Member            | Team        | Role(s)                            | Main Responsibilities                                                                 | Required Skills                        | Estimated Workload (%) |
| ---------------------- | ----------- | ---------------------------------- | ------------------------------------------------------------------------------------- | -------------------------------------- | ---------------------- |
| Trần Nguyễn Thái Bình  | Engineering | Project Owner, Backend Dev, DevOps | Backend, CI/CD, E2E, performance, infrastructure, business support                    | Backend dev, DevOps, business, testing | 20                     |
| Nguyễn Thái Gia Nguyễn | Engineering | Project Owner, Backend Dev         | Backend, API, integration, business support                                           | Backend dev, API, business             | 20                     |
| Trần Nguyễn Duy Minh   | Engineering | Frontend Dev                       | Frontend, E2E, UI, business support                                                   | Frontend dev, UI, business, testing    | 20                     |
| Đào Duy Vinh           | Engineering | Frontend Dev                       | Frontend, integration, UI, business support                                           | Frontend dev, integration, business    | 20                     |
| All Members            | Business    | Business Analyst, QA Engineer      | Requirement analysis, documentation, test planning, QA, bug reporting, business tasks | Analysis, documentation, QA, business  | 20                     |

## 4.3. Simple RACI Matrix

| Task / Deliverable    | Trần Nguyễn Thái Bình | Nguyễn Thái Gia Nguyễn | Trần Nguyễn Duy Minh | Đào Duy Vinh | All Members (Business Analyst, QA Engineer) | Informed (I)      |
| --------------------- | --------------------- | ---------------------- | -------------------- | ------------ | ------------------------------------------- | ----------------- |
| Requirement Gathering | A/R                   | C                      | C                    | C            | R                                           | All team, Sponsor |
| Backend Development   | A/R                   | R                      | C                    | C            | C                                           | All team, Sponsor |
| Frontend Development  | C                     | C                      | A/R                  | R            | C                                           | All team, Sponsor |
| Test Planning         | C                     | C                      | C                    | C            | A/R                                         | All team, Sponsor |
| CI/CD Setup           | A/R                   | R                      | C                    | C            | C                                           | All team          |
| E2E Testing           | C                     | R                      | R                    | C            | A                                           | All team, Sponsor |
| Documentation         | R                     | C                      | C                    | C            | A/R                                         | All team          |

**Legend:**  
A = Accountable, R = Responsible, C = Consulted, I = Informed

## 4.4. Assignment Adjustment Based on Actual Experience

| Team Member            | Initial Assignment            | Adjustment Reason             | Adjusted Assignment                                                     |
| ---------------------- | ----------------------------- | ----------------------------- | ----------------------------------------------------------------------- |
| Trần Nguyễn Thái Bình  | Backend, DevOps, CI/CD        | Strong DevOps experience      | Lead CI/CD and performance testing                                      |
| Nguyễn Thái Gia Nguyễn | Backend, API testing          | Deep API knowledge            | Focus on API and integration testing                                    |
| Trần Nguyễn Duy Minh   | Frontend, E2E testing         | Good at UI automation         | Lead E2E and component testing                                          |
| Đào Duy Vinh           | Frontend, integration testing | New to project, learning fast | Support UI and integration testing                                      |
| All Members            | Business/QA/BA roles          | Shared responsibility         | Lead documentation, requirement traceability, test planning, bug triage |

# 5. Communication Plan

| **Communication**        | **Recipient Groups**              | **Communication Time**                      | **Tool**                                      | **Goal**                                                                                   | **Owner**       |
| ------------------------ | --------------------------------- | ------------------------------------------- | --------------------------------------------- | ------------------------------------------------------------------------------------------ | --------------- |
| Project Kick-off Meeting | Core Team, All Stakeholders       | Once (Project start)                        | Google Meet                                   | Introduce project goals, objectives, scope timeline, deliverables & assign roles.          | Project Manager |
| Daily Stand-up Meeting   | Core Team                         | Daily                                       | In person (Mon - Fri), Google Meet (Sat, Sun) | For each member to dicuss their progress, identify problems.                               | Core Team       |
| Monthly Review           | Core Team, Stakeholders, Clients  | Monthly (1st day each month)                | Google Meet                                   | Provide stakeholders and clients with current project progress, discuss ongoing problems.  | Project Manager |
| UI/UX Design Review      | Designer, Front-end team, Clients | Once (after each design phase is completed) | E-mail.                                       | Give the Clients an opportunity to provide feedback on the design.                         | Designer        |
| Testing Review           | QA, Developer team, PM            | As much as needed during testing phase      | Github Issues / Google Meet                   | Review bugs and defects.                                                                   | QA              |
| Lessons Learned Meeting  | Core Team                         | End of Project                              | In person                                     | Assesses successes and failures during project, provide feedback for further improvements. | PM              |

# 6. Kick-off Meeting Minutes

## 6.1. Title

|                                             |            |
| ------------------------------------------- | ---------- |
| # **KICK-OFF**<br><br># **MEETING MINUTES** | Number: 01 |
| Issued Date: 01/09/2025                     |
| Page number:                                |

|                  |                            |              |         |
| ---------------- | -------------------------- | ------------ | ------- |
| Meeting Purpose  | Project kick-off meeting   |              |         |
| Meeting Location | Google Meet                |              |         |
| Meeting Date     | 01/09/2025                 | Meeting Time | 9:00 AM |
| Facilitator      | Trần Nguyễn Thái Bình (PM) |              |         |
| Project Name     | Electricilies              |              |         |

| ## Representatives |                        |                |      |
| ------------------ | ---------------------- | -------------- | ---- |
| No.                | Name                   | Role           | Note |
| 1                  | Trần Nguyễn Thái Bình  | PM             |      |
| 2                  | Nguyễn Thái Gia Nguyễn | Developer Team |      |
| 3                  | Trần Nguyễn Duy Minh   | Developer Team |      |
| 4                  | Đào Duy Vinh           | Developer Team |      |
| 5                  | \[Stakeholders\]       | Stakeholders   |      |

## 6.2. Project Introduction

- Electricilies is an e-commerce platform, designed to provide a comprehensive online marketplace to buy and sell electronic products. The system allows customers to browse products, manage their cart and purchase products with preferred payment methods.
- Electricilies also includes a CMS system for Administrators and Staff members to manage the website.

## 6.3. Project Objectives

- Aims to provide a user-friendly, responsive e-commerce system by the end of the project timeline (3 months).
- Includes secure payment gateway integration.
- Connects electronic providers to the system, allowing publishers to be updated with the project status monthly.

## 6.4. Methodology

- Development will follow the Incremental Model in the span of 3 months.
- Tools:
  - Jira: Task, backlog management
  - Github: version control system
  - Github Actions: CI/CD
  - Figma: UI/UX design

## 6.5. Team Roles

- Project Manager: Bình
- Designer: Minh, Vinh
- Front-end Dev Team: Minh, Vinh
- Back-end Dev Team: Binh, Nguyễn
- Testing Team:
  - Unit Testing & Integration Testing:
    - Front-end: Minh, Vinh
    - Back-end: Bình, Nguyễn
  - E2E Testing: Bình, Vinh

## 6.6. Stakeholder Questions

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

# 7. Appendix

## 7.1. Prompts

Below are prompts for corresponding sections

### 7.2. Budget Management

```markdown
I have given you context about my project including use cases, function list. You will create budget management in the bottom-up method for Electricilies - Website for Selling Electronic Products. This is just a university project, 4 members, so don't think this is for a big company. We use github and github action, deploy on selfhost kubernetes (not cloud), office at school or work from home, free document, grafana and prometheus stack, testing (Playwright, K6, Codecov, SonarQube)
```

### 7.3. Human Resource Management

```markdown
Create a resource management plan for a project (scope: all project activities, including business and engineering, not just testing).  
Follow these requirements:

1. Resource and Personnel Allocation Plan:
   - Present in a markdown table with columns: Resource Type, Description, Allocation Criteria, Allocation Plan.

2. Roles, Skills, and Workload Identification:
   - Present in a markdown table with columns: Team Member, Team, Role(s), Main Responsibilities, Required Skills, Actual Experience, Estimated Workload (%).
   - Note: Business Analyst and QA Engineer are not individual members; these are shared roles for all team members.

3. RACI Matrix:
   - List all team members and their teams above the table.
   - Present in a markdown table with columns: Task / Deliverable, [each team member], All Members (Business Analyst, QA Engineer), Informed (I).
   - Use A = Accountable, R = Responsible, C = Consulted, I = Informed.

4. Assignment Adjustment Based on Actual Experience:
   - Present in a markdown table with columns: Team Member, Initial Assignment, Adjustment Reason, Adjusted Assignment.

Write all content in English.  
Format all sections and tables in markdown.
```
