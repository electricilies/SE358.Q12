# Scrum

## Roles

- Trần Nguyễn Thái Bình: Product Owner, Scrum Master, DevOps Engineer, Backend Developer
- Nguyễn Thái Gia Nguyễn: Backend Developer
- Trần Nguyễn Duy Minh: Frontend Developer, Tester
- Đào Duy Vinh: Designer, Frontend Developer

# Sprint Backlog

## Daily scrum

### Mon 03 Nov 2025

#### Trần Nguyễn Thái Bình

- What did you do yesterday?
  - Set up the Kubernetes manifest for deployment
- What are you doing today?
  - Try to deploy the backend and frontend
  - Setting up the monitoring and auto scaling
- Is there anything blocking you?
  - Backend and frontend developers haven’t released any containers yet, so it's hard to test if the deployment environment works or not, need to ask them to release

#### Nguyễn Thái Gia Nguyễn

- What did you do yesterday?
  - Set up the CI workflow for frontend and backend repositories
- What are you doing today?
  - Set up Keycloak that provides the user management (sign-in, sign-up, ban, user profile management, password recovery,…)
  - Deploy the static swagger page for frontend team to know what are the models (DTOs) look like, help they code with the backend deployed
  - Ready to release the first version
- Is there anything blocking you?
  - The Domain Driven Design with Clean Architecture is so confusing, May refactor the code, which will slow down the progress
  - Keycloak client (GoCloak) doesn’t have well documentation, need to understand the logic of Keycloak including OAuth2 and OpenID Connect

#### Trần Nguyễn Duy Minh

- What did you do yesterday?
  - Set up authentication for the frontend app, connect Keycloak to AuthJS
- What are you doing today?
  - Implement the signin/signup screen
  - Initial release the frontend
- Is there anything blocking you?
  - The backend team hasn't deployed yet, so I can just mock the request/data to retrieve products based on the Swagger the backend team gave
  - Have to read the AuthJS documentation, which is currently unmaintained and merged into BetterAuth

#### Đào Duy Vinh

- What did you do yesterday?
  - Designed the Authentication Screen (Signin, Signup)
- What are you doing today?
  - Adding more fields while registering a user (address, phone number)
  - Design the user profile management screen

### Tue 04 Nov 2025

#### Trần Nguyễn Thái Bình

- What did you do yesterday?
  - Successfully deployed both backend and frontend to the dev environment deployment
  - Done setting up monitoring and autoscaling
- What are you doing today?
  - Join the backend team to implement, handle the event user registration from Keycloak into Kafka for the backend to consume later (creating users' carts in the future)
- Is there anything blocking you?
  - I have to learn the architecture of the backend (Domain Driven Design + Clean Architecture)

#### Nguyễn Thái Gia Nguyễn

- What did you do yesterday?
  - Released the first container image
- What are you doing today?
  - Integrated Keycloak authentication middleware into the backend
  - Set up role middleware to use in the future
- Is there anything blocking you?
  - No library suits our needs, so I have to implement the middleware myself

#### Trần Nguyễn Duy Minh

- What did you do yesterday?
  - Implemented home screen
  - Released the first container image
- What are you doing today?
  - Found a perf issue, need to add debounce in the typing fields
  - Implement the user management profile screen (editing profile, delete account)
- Is there anything blocking you?
  - CI failed to release the container due to a Thái Bình’s mistake in declaring CI pipeline, so I had to wait for him to fix it

#### Đào Duy Vinh

- What did you do yesterday?
  - Designed the user management screen
- What are you doing today?
  - Help integrating third paty provider to Keycloak (Google, Github)
- Is there anything blocking you?
  - Have to read Keycloak integration, and how to integrate Google, Github identity provider to Keycloak

---

# **Sprint Review**

## **Sprint Goals**

- Deploy backend and frontend services to the development environment using Kubernetes.
- Integrate Keycloak for authentication, user management, and third-party identity providers
- Release the first backend and frontend container images
- Set up CI/CD pipelines
- Begin frontend–backend integration with Swagger documentation and mock data.
- Design and implement authentication and user profile UI screens.

---

## **Completed Work**

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

---

## **Incomplete or Deferred Work**

- Backend architecture (DDD + Clean Architecture) still requires minor learning for some team members.
- Need more time for the integration of Google/GitHub identity providers with Keycloak.

---

## **Demo Summary**

- Showed successful deployment of backend and frontend in Kubernetes.
- Showed authentication flow using Keycloak (signin, signup, protected routes).
- Presented Swagger API documentation.
- Showed initial UI designs and implemented authentication screens.
- Discussed backend architecture complexity and issues with Keycloak libraries.

---

## **Stakeholder Feedback**

- Stakeholders acknowledged major progress in setting up authentication and deployment infrastructure.
- Requested faster collaboration between backend and frontend teams to reduce mock-based APIs.
- Encouraged continued improvements in API completeness and documentation.

---

# **Sprint Retrospective**

## **What went well**

- Strong team collaboration between team members.
- Deployed Backend and frontend to the dev environment.
- Set up CI/CD pipelines.
- Finished setting up Keycloak for user authentication.
- Implemented authentication screens.
- Released first container images for both frontend and backend.

---

## **What could have been better**

- Backend complexity slowed implementation and require additional learning.
- Keycloak Go client (GoCloak) lacked some documentation so need further research.
- Slow designs due to designers not used to mock-up designs

---

## **What we will do differently**

- Define clear deadlines for image releases in order not to block tasks.
- Increase short meetings to quickly resolve integration issues.
- Improve documentation of backend architecture and API for better understanding.
- Standardize design documentation templates for clearer communication between designers and clients.

---

# **Individual Contributions and Observations**

### **Trần Nguyễn Thái Bình**

**Deliverables:** Kubernetes manifests, CI/CD setup, DevOps deployment, monitoring & autoscaling, support for backend integration.  
**Assessment:** Lead DevOps work and helped backend implementation. Also resolved CI/CD issues. Recommended to continue documentation and support the backend team.

### **Nguyễn Thái Gia Nguyễn**

**Deliverables:** CI/CD setup, Keycloak backend integration, initial backend container release, Swagger deployment.  
**Assessment:** Completed core authentication infrastructure. Recommended to continue API documentation.

### **Trần Nguyễn Duy Minh**

**Deliverables:** Frontend authentication flow using AuthJS + Keycloak, home screen implementation, first frontend container release, develop profile screen.  
**Assessment:** Actively address issues faced and successfully completed initial authentication screens.

### **Đào Duy Vinh**

**Deliverables:** Authentication and profile UI designs, support for frontend implementation, researching Keycloak third-party providers.  
**Assessment:** Designed clear UI and assisted the frontend team. Hard-worked in learning React/NextJS, should continue asking other members in case of blockers.
