# Scrum

## Roles

- Trần Nguyễn Thái Bình: Product Owner, Scrum Master, DevOps Engineer, Backend Developer
- Nguyễn Thái Gia Nguyễn: Backend Developer
- Trần Nguyễn Duy Minh: Frontend Developer, Tester
- Đào Duy Vinh: Designer, Frontend Developer

# Sprint Backlog

[https://electricilies.atlassian.net/issues/?jql=type in (Task, Subtask) ORDER BY created DESC](https://electricilies.atlassian.net/issues/?jql=type%20in%20(Task%2C%20Subtask)%20ORDER%20BY%20created%20DESC)

## Daily scrum

### Mon 03 Nov 2025

#### Trần Nguyễn Thái Bình

- What did you do yesterday?
  - Set up the Kubernetes manifest for deployment
  - Set up the CI workflow for frontend and backend repositories
- What are you doing today?
  - Try to deploy the backend and frontend
  - Setting up the monitoring and auto scaling
- Is there anything blocking you?
  - Backend and frontend developers haven’t released any containers yet, so it's hard to test whether the deployment environment works or not, need to ask them to release

#### Nguyễn Thái Gia Nguyễn

- What did you do yesterday?
  - Set up Keycloak that provides the user management (sign-in, sign-up, ban, user profile management, password recovery,…)
  - Integrated Keycloak authentication middleware into the backend
  - Deployed the static swagger page for frontend team to know what are the models (DTOs) look like, help they code with the backend deployed
- What are you doing today?
  - Implement product API (including CRUD)
  - Implement cart, payment API
  - Ready to release the first version
- Is there anything blocking you?
  - The Domain Driven Design with Clean Architecture is so confusing, May refactor the code, which will slow down the progress

#### Trần Nguyễn Duy Minh

- What did you do yesterday?
  - Set up authentication for the frontend app, and ensure the user signs in to access some protected pages
  - Add product pages (create, edit products for staff/admin)
- What are you doing today?
  - Implement home view (including listing product with suggested category)
  - Implement product detail screen
  - Implement review section for product detail screen
  - Implement review management screen
- Is there anything blocking you?
  - The backend team hasn't deployed yet, so I can just mock the request/data to retrieve products based on the Swagger the backend team gave

#### Đào Duy Vinh

- What did you do yesterday?
  - Told Duy Minh about the product screen (including home screen, search screen, product detail screen)
  - Designed the cart screen, payment screen, and documentation screen
- What are you doing today?
  - Help Duy Minh implement the cart screen, payment screen

### Tue 04 Nov 2025

#### Trần Nguyễn Thái Bình

- What did you do yesterday?
  - Successfully deployed both backend and frontend to the dev environment deployment
  - Done setting up monitoring and autoscaling
- What are you doing today?
  - Join the backend team to implement the documentation API (including code and additional SQL because backend team hasn’t code the SQL yet)
  - Add missing SQL trigger for updating product price when product variants' prices change
- Is there anything blocking you?
  - I have to learn the architecture of the backend (Domain Driven Design + Clean Architecture)

#### Nguyễn Thái Gia Nguyễn

- What did you do yesterday?
  - Implemented product API
  - Implemented cart API
  - Implemented the payment API, but only integrated VNPAY for now
  - Released the first container image
- What are you doing today?
  - Implement the search, sort, and filter ability for the product API
  - Implement review API
  - Integrate caching for product API (list products and get product)
- Is there anything blocking you?
  - Go library for VNPAY is not really documented and well-maintained
  - Handling database transactions in the flow of product creation is hard

#### Trần Nguyễn Duy Minh

- What did you do yesterday?
  - Implemented home screen
  - Released the first container image
- What are you doing today?
  - Found a perf issue in …, have to fix that \----------------
  - Implement ……….
- Is there anything blocking you?
  - CI failed to release the container due to a Thái Bình’s mistake in declaring CI pipeline, so I had to wait for him to fix it
  - Have to read how the presign URL works to upload and delete images (in product and review)

#### Đào Duy Vinh

- What did you do yesterday?
  - Implemented the cart screen
  - Implemented the payment screen

- What are you doing today?

- Is there anything blocking you?
  - Have to review how to code NextJS and React

# Sprint Review

## Sprint Goals

- Deploy backend and frontend services to the development environment using Kubernetes.
- Implement core authentication and user management features.
- Deliver initial product, cart, and payment APIs.
- Release first container images for backend and frontend.
- Begin frontend integration with backend APIs and mock data.
- Design and implement key UI screens: home, product detail, cart, payment, and review management.

## Completed Work

- Kubernetes manifests and CI workflows set up for deployment.
- Backend and frontend successfully deployed to dev environment.
- Keycloak integrated for user authentication and management.
- Swagger documentation published for API models.
- Product, cart, and payment APIs implemented (VNPay integrated).
- First backend and frontend container images released.
- Frontend authentication and protected routes established.
- Home, product, cart, payment, and review screens designed and partially implemented.
- Monitoring and autoscaling configured for deployments.

## Incomplete or Deferred Work

- Some backend APIs (search, sort, filter, review) are still in progress.
- SQL triggers and documentation API require further development.
- Frontend integration with live backend data is limited; some features use mocked data.
- Review management and image upload (presign URL) need additional work.

## Demo Summary

- Team demonstrated deployment of backend and frontend services.
- Showed authentication flow and product management screens.
- Presented initial API endpoints and frontend integration.
- Discussed challenges with backend architecture and third-party libraries.

## Stakeholder Feedback

- Stakeholders acknowledged progress on deployment and core features.
- Requested continued focus on API completeness and frontend-backend integration.
- Emphasized importance of timely releases and documentation updates.

# Sprint Retrospective

## What went well

- Team members collaborated effectively across backend, frontend, and DevOps roles, showing responsibility for assigned tasks.
- Successful deployment of backend and frontend services to the development environment using Kubernetes.
- CI/CD pipelines were set up, enabling faster integration and testing.
- Key authentication and user management features were implemented using Keycloak.
- Initial container images for backend and frontend were released, supporting further development and integration.

## What could have been better

- Coordination between backend and frontend releases was sometimes delayed, impacting deployment testing and integration.
- Some backend APIs (search, sort, filter, review) and database logic (SQL triggers) were slower to implement due to architectural complexity.
- CI pipeline errors temporarily blocked frontend container release, requiring additional troubleshooting.
- Documentation API and image upload integration (presign URL) need further attention to improve usability and traceability.

## What will we do differently

- Set clear deadlines for container image delivery to improve release coordination between backend and frontend teams.
- Schedule regular syncs to quickly resolve integration blockers and ensure timely progress updates.
- Document architectural decisions and API changes to reduce confusion and rework.
- Assign backup owners for CI/CD and deployment tasks to avoid bottlenecks and ensure continuity.

## Individual contributions and observations

- Trần Nguyễn Thái Bình
  - Deliverables: Kubernetes manifests, CI/CD setup, deployment of backend and frontend, support for backend API development.
  - Assessment: Led DevOps efforts and resolved CI/CD issues. Supported backend team with documentation API and SQL triggers. Recommend continued attention to deployment coordination and documentation.
- Nguyễn Thái Gia Nguyễn
  - Deliverables: Key backend APIs (product, cart, payment), integration of Keycloak, release of backend container image.
  - Assessment: Delivered core backend features and overcame challenges with third-party libraries and database transactions. Recommend documenting architectural decisions and external tool usage for future reference.
- Trần Nguyễn Duy Minh
  - Deliverables: Frontend authentication, product management screens, release of frontend container image.
  - Assessment: Implemented key frontend features and adapted to backend delays by using mock data. Resolved CI issues and contributed to integration efforts. Recommend maintaining thorough documentation and timely publication of deliverables.
- Đào Duy Vinh
  - Deliverables: UI design for cart, payment, and documentation screens; support for frontend development.
  - Assessment: Designed and implemented UI screens, supported frontend team, and continued learning NextJS and React. Recommend adopting team templates for design documentation and sharing updates regularly.