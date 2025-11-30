# 1. Mini-sprint Scrum

## 1.1. Roles

- Trần Nguyễn Thái Bình: Product Owner, Scrum Master, DevOps Engineer, Backend Developer
- Nguyễn Thái Gia Nguyễn: Backend Developer
- Trần Nguyễn Duy Minh: Frontend Developer, Tester
- Đào Duy Vinh: Designer, Frontend Developer

## 1.2. Sprint Backlog

## 1.3. Daily scrum

### 1.3.1. Mon 03 Nov 2025

#### 1.3.1.1. Trần Nguyễn Thái Bình

- What did you do yesterday?
  - Set up the Kubernetes manifest for deployment
- What are you doing today?
  - Try to deploy the backend and frontend
  - Setting up the monitoring and auto scaling
- Is there anything blocking you?
  - Backend and frontend developers haven’t released any containers yet, so it's hard to test if the deployment environment works or not, need to ask them to release

#### 1.3.1.2. Nguyễn Thái Gia Nguyễn

- What did you do yesterday?
  - Set up the CI workflow for frontend and backend repositories
- What are you doing today?
  - Set up Keycloak that provides the user management (sign-in, sign-up, ban, user profile management, password recovery,…)
  - Deploy the static swagger page for frontend team to know what are the models (DTOs) look like, help they code with the backend deployed
  - Ready to release the first version
- Is there anything blocking you?
  - The Domain Driven Design with Clean Architecture is so confusing, May refactor the code, which will slow down the progress
  - Keycloak client (GoCloak) doesn’t have well documentation, need to understand the logic of Keycloak including OAuth2 and OpenID Connect

#### 1.3.1.3. Trần Nguyễn Duy Minh

- What did you do yesterday?
  - Set up authentication for the frontend app, connect Keycloak to AuthJS
- What are you doing today?
  - Implement the signin/signup screen
  - Initial release the frontend
- Is there anything blocking you?
  - The backend team hasn't deployed yet, so I can just mock the request/data to retrieve products based on the Swagger the backend team gave
  - Have to read the AuthJS documentation, which is currently unmaintained and merged into BetterAuth

#### 1.3.1.4. Đào Duy Vinh

- What did you do yesterday?
  - Designed the Authentication Screen (Signin, Signup)
- What are you doing today?
  - Adding more fields while registering a user (address, phone number)
  - Design the user profile management screen

### 1.3.2. Tue 04 Nov 2025

#### 1.3.2.1. Trần Nguyễn Thái Bình

- What did you do yesterday?
  - Successfully deployed both backend and frontend to the dev environment deployment
  - Done setting up monitoring and autoscaling
- What are you doing today?
  - Join the backend team to implement, handle the event user registration from Keycloak into Kafka for the backend to consume later (creating users' carts in the future)
- Is there anything blocking you?
  - I have to learn the architecture of the backend (Domain Driven Design + Clean Architecture)

#### 1.3.2.2. Nguyễn Thái Gia Nguyễn

- What did you do yesterday?
  - Released the first container image
- What are you doing today?
  - Integrated Keycloak authentication middleware into the backend
  - Set up role middleware to use in the future
- Is there anything blocking you?
  - No library suits our needs, so I have to implement the middleware myself

#### 1.3.2.3. Trần Nguyễn Duy Minh

- What did you do yesterday?
  - Implemented home screen
  - Released the first container image
- What are you doing today?
  - Found a perf issue, need to add debounce in the typing fields
  - Implement the user management profile screen (editing profile, delete account)
- Is there anything blocking you?
  - CI failed to release the container due to a Thái Bình’s mistake in declaring CI pipeline, so I had to wait for him to fix it

#### 1.3.2.4. Đào Duy Vinh

- What did you do yesterday?
  - Designed the user management screen
- What are you doing today?
  - Help integrating third paty provider to Keycloak (Google, Github)
- Is there anything blocking you?
  - Have to read Keycloak integration, and how to integrate Google, Github identity provider to Keycloak

## 1.4. Sprint Review

### 1.4.1. Sprint Goals

- Deploy backend and frontend services to the development environment using Kubernetes.
- Integrate Keycloak for authentication, user management, and third-party identity providers
- Release the first backend and frontend container images
- Set up CI/CD pipelines
- Begin frontend–backend integration with Swagger documentation and mock data.
- Design and implement authentication and user profile UI screens.

### 1.4.2. Completed Work

- Kubernetes manifests created and Dev environment successfully deployed for backend and frontend.
- Set up CI workflows for backend and frontend
- Release first version of backend and frontend container.
- Keycloak integrated with backend (authentication middleware, role middleware) and frontend (AuthJS).
- Deployed Static Swagger documentation.
- Configured monitoring and autoscaling in Kubernetes.
- Finished authentication screens (signin/signup).
- Set up authentication flow with protected routes.
- Designed initial user profile management screen.
- Keycloak event handling planned for future user features (e.g., cart,…).

### 1.4.3. Incomplete or Deferred Work

- Backend architecture (DDD + Clean Architecture) still requires minor learning for some team members.
- Need more time for the integration of Google/GitHub identity providers with Keycloak.

### 1.4.4. Demo Summary

- Showed successful deployment of backend and frontend in Kubernetes.
- Showed authentication flow using Keycloak (signin, signup, protected routes).
- Presented Swagger API documentation.
- Showed initial UI designs and implemented authentication screens.
- Discussed backend architecture complexity and issues with Keycloak libraries.

### 1.4.5. Stakeholder Feedback

- Stakeholders acknowledged major progress in setting up authentication and deployment infrastructure.
- Requested faster collaboration between backend and frontend teams to reduce mock-based APIs.
- Encouraged continued improvements in API completeness and documentation.

## 1.5. Sprint Retrospective

### 1.5.1 What went well

- Strong team collaboration between team members.
- Deployed Backend and frontend to the dev environment.
- Set up CI/CD pipelines.
- Finished setting up Keycloak for user authentication.
- Implemented authentication screens.
- Released first container images for both frontend and backend.

### 1.5.2. What could have been better

- Backend complexity slowed implementation and require additional learning.
- Keycloak Go client (GoCloak) lacked some documentation so need further research.
- Slow designs due to designers not used to mock-up designs

### 1.5.3. What will we do differently

- Define clear deadlines for image releases in order not to block tasks.
- Increase short meetings to quickly resolve integration issues.
- Improve documentation of backend architecture and API for better understanding.
- Standardize design documentation templates for clearer communication between designers and clients.

### 1.5.4. Individual contributions and observations

- Trần Nguyễn Thái Bình
  - Deliverables: Kubernetes manifests, CI/CD setup, DevOps deployment, monitoring & autoscaling, support for backend integration.
  - Assessment: Lead DevOps work and helped backend implementation. Also resolved CI/CD issues. Recommended to continue documentation and support the backend team.

- Nguyễn Thái Gia Nguyễn
  - Deliverables: CI/CD setup, Keycloak backend integration, initial backend container release, Swagger deployment.
  - Assessment: Completed core authentication infrastructure. Recommended to continue API documentation.

- Trần Nguyễn Duy Minh
  - Deliverables: Frontend authentication flow using AuthJS + Keycloak, home screen implementation, first frontend container release, develop profile screen.
  - Assessment: Actively address issues faced and successfully completed initial authentication screens.

- Đào Duy Vinh
  - Deliverables: Authentication and profile UI designs, support for frontend implementation, researching Keycloak third-party providers.
  - Assessment: Designed clear UI and assisted the frontend team. Hard-worked in learning React/NextJS, should continue asking other members in case of blockers.

# 2. Agile vs Waterfall

# 2.1. Case Study: eCommerce Website for Electronic Products (Electricilies)

## 2.1.1. Overview

Electricilies is an online eCommerce platform for electronic products. This project is expected to be done in 12 weeks and must have the main functions which allows the customers to:

- View all products on the product listing page, allows keyword searching as well as sort options.
- Manage their carts, including adding a product to cart, adjust product quantity in cart, and remove products from their cart.
- Add delivery address for shipping (part of the checkout process)
- Choose suitable payment options, notably online payment.

The platform must also include a CMS (Content Management System) site for internal staff to manage the website.

## 2.1.2. Main Modules

Website contains these main modules:

- Module 1: Authentication & Authorization (Register, Login,…)
- Module 2: Product & Product Details
- Module 3: Cart
- Module 4: Checkout & Payment
- Module 5: Blog & Articles
- Module 6: Content Management System

## 2.1.3. Agile vs. Waterfall Methodologies

| ## **Agile**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | ## **Waterfall**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ### 1\. Project Progress Plan                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Agile divides the project into 6 **sprints**, each lasting **2 weeks:**<br><br>#### 1\. Sprint 1 - Authentication & Authorization<br><br>**Objectives:**<br><br>- Allows user to register and login through the system using JWT<br>- Session management<br>- Reset password by sending confirmation emails.<br>- Separate customer, staff, admin roles and permissions<br><br>**Deliverables:**<br><br>- Register and login page<br>- Redirect correspondingly according to user roles<br><br>#### 2\. Sprint 2 - Product & Product Details<br><br>**Objectives**<br><br>- Allows customers to view product listing and product details<br>- Allows staff to add products<br>- Search function and sorting options<br><br>**Deliverables**<br><br>- Product listing page with searching<br>- Product details page<br>- Product management page in CMS<br><br>#### 3\. Sprint 3 - Cart<br><br>**Objectives**<br><br>- Allows customer to add or remove products in cart, adjust product quantities<br>- Display cart subtotal correspondingly<br><br>**Deliverables**<br><br>- Cart page with data synced to each customer<br><br>#### 4\. Sprint 4 - Checkout & Payment<br><br>**Objectives**<br><br>- Allows customer to enter their shipping address<br>- Allows customer to choose payment options<br>- Integrate third party Payment Gateway service<br>- Create order after payment<br><br>**Deliverables**<br><br>- Shipping page with information form<br>- Payment page with redirection to third party payment site, complete payment flow<br>- Order management page in CMS<br><br>#### 5\. Sprint 5 - Blog & Articles<br><br>**Objectives**<br><br>- Allows customer to browse the blog page for articles, view articles content<br><br>**Deliverables**<br><br>- Blog page, article details view page<br>- Article management page in CMS<br><br>#### 6\. Sprint 6 - Optimization & Monitoring<br><br>**Objectives**<br><br>- Optimize leftover issues from previous stages<br>- Performance monitoring (linked with third party services like Grafana)<br>- Sales report stats<br>- Document writeup<br><br>**Deliverables**<br><br>- CMS Dashboard with sales report and performance monitoring<br>- Documents related to the project and instructions manual for the whole system<br>- Fully operational system | Waterfall divides the project into 5 separate stages:<br><br>#### 1\. Requirement Specification - 3 weeks<br><br>- Do market research, interview with clients and stakeholders<br>- Define project scope, functional and non-functional requirements<br>- Write an SRS document<br><br>#### 2\. Project Design - 2 weeks<br><br>- Design overall system architecture<br>- Build website’s UI/UX<br>- Define ERD, create database schema<br><br>#### 3\. Development - 5 weeks<br><br>Code all modules of the system following initial requirements defined in previous stage’s documents<br><br>Frontend:<br><br>- Product pages (7 days)<br>- Cart & Checkout pages (4 days)<br>- Profile pages (3 days)<br>- Blog pages (4 days)<br>- CMS pages (17 days)<br><br>Backend:<br><br>- Account & Authentication API (7 days)<br>- User Management API (5 days)<br>- Product API (7 days)<br>- Payment API (3 days)<br>- Order API (4 days)<br>- Document API (4 days)<br>- System Monitoring (5 days)<br><br>#### 4\. Testing - 1 week<br><br>- API testing<br>- UI, Integration testing<br><br>#### 5\. Document Writeup - 1 week |
| ### 2\. Planning Strategy                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| - Planning is done at the start of each Sprint (1-6), and only for that corresponding Sprint.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | - Planning is done at the start of the whole project, and often never changes during the project.<br>- However, Clients often find it difficult to outline all their requirements at the beginning, which often leads to gaps in documentation.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ### 3\. Flexibility to Changes<br><br>Assuming **during the project,** our Client wants to implement a **Filtering function** to the system.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| - Team actively discusses with Client about the function requirements, etc…<br>- All works related to the function is added to the **Backlog**, and will be handled in the Sprint after.<br>- Moreover, frequent feedback is encouraged which brings higher customer satisfaction and further satisfy their needs.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | - Due to planning is already done at the start, all requirements and functions have been specified, changes during the project are never possible in most cases.<br>- In some cases backtracking to the previous phases for that single function is possible, however, Waterfall is a **sequential model** in nature so revisiting previous phases is not only very costly but also produce more risks.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ### 4\. Risk Of Delays                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| - Testing is done at the end of each Sprint, therefore if defects are found in the system, additional tasks can be comfortably added to the Backlog and will be handled after.<br>- If any task does not meet deadline due to unforeseen circumstances, the Backlog can be adjusted adaptively.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | - Testing is done near the end of the project, therefore if defects are found, it is often costly to fix and can lead to delays in progress.<br>- If any module does not meet its pre-defined deadline, modules following after will also be delayed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ### 5\. Tracking & Controlling Progress                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| - Holds a 10-15 minutes daily stand up everyday in which every member discusses:<br> - What I did yesterday?<br> - What will I do today?<br> - What issues am I having?<br>- Close collaboration between team members mean that raised issues can be solved within a short time.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | - Collaboration or Communication is often formal and based on documents.<br>- Use key milestones in stages to track progress (example: SRS completed, Design completed, Development completed,…)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

## 2.1.4. Model Choice

That being said, our team chooses the **Waterfall Model** for our project due to the following reasons:

- Our scope is relatively small, with only 6 modules which can be planned linearly.
- For this project, the requirements are fixed beforehand so requirement changes during the project is highly unlikely.
- Our team has a small size of 4 members, and all of our roles are fixed throughout the project. Each member is specialized in a role.

However, our team often holds occasional meetings to discuss progress and address issues that each member is facing. In the case of further development such as expanding scope, adding modules, our team could adapt to the Incremental Model.

# 3. Retrospective

## 3.1. What went well

- Most members worked well together and interacted actively, except for Đào Duy Vinh who had personal matters.
- During the SCRUM meetings, members started coding right away. Everyone supported each other and divided tasks reasonably.
- Gained a clearer understanding of the Waterfall and Agile models, along with their pros and cons.

## 3.2. What could have been better

- Finishing more tasks in one sprint to use our time better and complete the product faster.
- Holding SCRUM meetings at a time when all members can join.

## 3.3. What will we do differently

- In the next sprint, complete the "product" module in addition to the "Manage User" module.
- Announce the meeting schedule 2 days in advance instead of on the same day, so everyone can arrange their time properly.
- Consider upgrading to NextJS 16, use BetterAuth instead of AuthJS which is deprecated and merged into BetterAuth.

## 3.4. Individual contributions and observations

- Trần Nguyễn Duy Minh, Đào Duy Vinh
  - Deliverables: Agile vs Waterfall, SCRUM meeting, Frontend code
  - Assessment: Did very well
  - Recommendation: Consider combining both Waterfall and Agile models in software development

- Trần Nguyễn Duy Minh, Đào Duy Vinh
  - Deliverables: Agile vs Waterfall, SCRUM meeting, design
  - Assessment: Work was uneven; Vinh was busy with personal matters, so Minh had to handle most of the workload

- Trần Nguyễn Thái Bình
  - Deliverables: SCRUM meeting, DevOps code
  - Assessment: Good at organizing meetings and handling infrastructure issues
  - Recommendation: Should ask Nguyễn and other members for opinions before making decisions

- Nguyễn Thái Gia Nguyễn
  - Deliverables: SCRUM meeting, Backend code
  - Assessment: Supported Bình in running meetings and coordinated well between members during the coding process
