# 1. Project Closure

**Project Name:** Electricilies – Website for Selling Electronic Products

## 1.1. Document Control

### 1.1.1. Document Information

|                     |                                        |
| ------------------- | -------------------------------------- |
| **Document Id**     | ELEC-CLOSE-001                         |
| **Document Owner**  | Trần Nguyễn Thái Bình                  |
| **Issue Date**      | 2025-11-28                             |
| **Last Saved Date** | 2025-11-28                             |
| **File Name**       | Project Closure Report - Electricilies |

### 1.1.2. Document Approvals

| **Role**              | **Name**              | **Date**   |
| --------------------- | --------------------- | ---------- |
| **Lecturer**          | Lê Văn Tuấn           | 2025-11-28 |
| **Project Manager**   | Trần Nguyễn Thái Bình | 2025-11-28 |
| **Quality Assurance** | Trần Nguyễn Duy Minh  | 2025-11-28 |

## 1.2. Project Completion

This section identifies the criteria required to complete the project and any outstanding items which still need to be undertaken.

### 1.2.1. Completion Criteria

| **Category**     | **Criteria**                                                                        | **Achieved** |
| ---------------- | ----------------------------------------------------------------------------------- | ------------ |
| **Objectives**   | Develop a user-friendly website for browsing and purchasing electronic products.    | **Yes**      |
|                  | Implement secure authentication (Keycloak) and payment integration (VNPay).         | **Yes**      |
|                  | Create an admin interface for product and order management.                         | **Yes**      |
| **Benefits**     | Platform supports retail and wholesale customers with seamless shopping experience. | **Yes**      |
|                  | System handles high concurrency via Kubernetes autoscaling.                         | **Yes**      |
| **Deliverables** | Fully functional source code (Frontend/Backend) deployed on K8s.                    | **Yes**      |
|                  | Comprehensive documentation (Architecture, API Swagger, User Manuals).              | **Yes**      |
|                  | Test Reports (Unit, Integration, E2E) with >80% coverage.                           | **Yes**      |

### 1.2.2. Outstanding Items

List of items that remain incomplete or require further attention after project closure.

| **Item**          | **Action**                                                                    | **Owner**              |
| ----------------- | ----------------------------------------------------------------------------- | ---------------------- |
| **Backend API**   | Finalize advanced Search, Sort, and Filter logic for large datasets.          | Nguyễn Thái Gia Nguyễn |
| **Image Upload**  | Fix Presigned URL generation logic for product image uploads in CMS.          | Trần Nguyễn Duy Minh   |
| **Documentation** | Update API documentation to reflect the latest changes in the Review Module.  | Trần Nguyễn Thái Bình  |
| **Security**      | Conduct final penetration testing on the payment gateway integration sandbox. | Trần Nguyễn Thái Bình  |

## 1.3. Project Closure

This section outlines the handover of deliverables, documentation, resources, and communication.

### 1.3.1. Deliverables Handover

| **Deliverable**    | **Current Owner** | **Current Location**     | **New Owner**    | **Handover Activities**                                | **Date**   |
| ------------------ | ----------------- | ------------------------ | ---------------- | ------------------------------------------------------ | ---------- |
| **Source Code**    | Dev Team          | GitHub (Private Repo)    | Maintenance Team | Transfer repository ownership; Grant admin access.     | 2025-11-30 |
| **Infrastructure** | DevOps (Bình)     | Self-hosted K8s Cluster  | Ops Team         | Transfer SSH keys; Hand over `kubeconfig` and secrets. | 2025-11-30 |
| **Database**       | Backend Team      | PostgreSQL (Self-hosted) | Ops Team         | Provide connection strings; Verify backup integrity.   | 2025-11-30 |

### 1.3.2. Documentation Handover

| **Documentation**     | **Current Owner** | **Current Location**      | **New Owner**       | **Handover Activities**                             | **Date**   |
| --------------------- | ----------------- | ------------------------- | ------------------- | --------------------------------------------------- | ---------- |
| **Project Artifacts** | PM (Bình)         | Confluence / Google Drive | Client / Lecturer   | Archive Phase A-D reports; Export to PDF.           | 2025-11-29 |
| **Technical Docs**    | Dev Team          | GitHub Wiki / VitePress   | Maintenance Team    | Publish final API Swagger; Update deployment guide. | 2025-11-29 |
| **Design Assets**     | Designers         | Figma                     | Marketing / UI Team | Share "View/Edit" access to final design files.     | 2025-11-29 |

### 1.3.3. Suppliers

| **Supplier Name**   | **Contract Reference** | **Termination Activity**                            | **Release Date** | **Activity Owner**     |
| ------------------- | ---------------------- | --------------------------------------------------- | ---------------- | ---------------------- |
| **VNPay**           | Sandbox Integration    | Switch to Production Mode or Close Sandbox Account. | 2025-12-01       | Nguyễn Thái Gia Nguyễn |
| **Domain Provider** | .id.vn Registration    | Transfer domain management credentials to Client.   | 2025-12-01       | Trần Nguyễn Thái Bình  |

### 1.3.4. Resources

| **Resource Name**    | **Current Designation** | **Release Activity**                                       | **Release Date** | **Activity Owner**    |
| -------------------- | ----------------------- | ---------------------------------------------------------- | ---------------- | --------------------- |
| **Dev Team Members** | Developers / QA         | Release to other academic courses; Conduct exit interview. | 2025-11-30       | Trần Nguyễn Thái Bình |
| **Mini PC Server**   | K8s Master Node         | Wipe sensitive data; Return hardware to Lab/Owner.         | 2025-12-05       | Trần Nguyễn Thái Bình |
| **Network Switch**   | Infrastructure          | Disconnect and return to inventory.                        | 2025-12-05       | Trần Nguyễn Thái Bình |

### 1.3.5. Communication

| **Target Audience**    | **Intended Message**                                                  | **Method Used**                | **Dispatch Date** | **Dispatch Owner**    |
| ---------------------- | --------------------------------------------------------------------- | ------------------------------ | ----------------- | --------------------- |
| **Lecturer / Sponsor** | Project successfully completed; Final Report submitted.               | Email & In-person Presentation | 2025-11-28        | Trần Nguyễn Thái Bình |
| **Development Team**   | Project closed; Thank you for contributions; Lessons learned session. | Team Meeting (Retrospective)   | 2025-11-29        | Trần Nguyễn Thái Bình |
| **End Users**          | Website is live (Beta version); Feedback channel open.                | Website Banner / Email         | 2025-12-01        | Đào Duy Vinh          |

## 1.4. Approval

**Name:** Trần Nguyễn Thái Bình

**Role:** Project Manager

**Signature:** _\[Signed\]_

**Date:** 28 / 11 / 2025

By signing this document, I grant approval to formally close this project and complete the hand-over activities as described above.

# 2. Lessons Learned – Electricilies Project

## 2.1. What We Learned

- **Collaboration & Responsibility:** Team members generally worked well together, showing responsibility for assigned tasks. Using Atlassian Confluence and Jira improved transparency and traceability.
- **Documentation:** Centralizing documents in Confluence made it easier to track changes and share information. However, some deliverables were published late, affecting traceability.
- **CI/CD & DevOps:** Setting up CI/CD pipelines and deploying on self-hosted Kubernetes taught us practical DevOps skills. We learned the importance of environment parity and monitoring.
- **Task Assignment & Progress Tracking:** Delays in initial task assignment and lack of a deputy lead slowed early progress. Not enforcing deadlines and milestone checks led to late deliveries.
- **Technical Challenges:** Integrating third-party tools (Keycloak, VNPay) and handling backend architectural complexity (DDD, Clean Architecture) required extra effort and learning.
- **Testing & Quality:** Automated testing (Playwright, K6, Codecov) and monitoring (Prometheus/Grafana) helped us meet quality targets, but some APIs and features were slower to complete due to unclear requirements or technical blockers.
- **Communication:** Daily stand-ups and regular meetings helped surface blockers, but inconsistent progress monitoring and unclear ownership sometimes caused bottlenecks.

## 2.2. Honest Reflections

- We underestimated the time needed for some tasks, especially backend API development and integration. This led to delays and required rework.
- Not having a backup lead meant decisions stalled when the main lead was unavailable.
- Some team members struggled with new technologies (Kubernetes, CI/CD, NextJS), but adapted by learning on the job and supporting each other.
- Deliverables were sometimes completed but not published promptly, reducing visibility for reviewers and stakeholders.
- Documentation templates and publication timelines were not standardized early enough, causing confusion.

## 2.3. Commitment

We commit to applying these lessons and improvement actions in future projects to deliver higher quality, maintain better traceability, and foster a more resilient, collaborative team.

# 3. Retrospective

## 3.1. What went well

- Completed all course tasks successfully
- Delivered all required artifacts for the course
- Understood how to manage a project and keep it stable and successful, including interacting with the team, human resources, customers, and other stakeholders
- Used online samples and AI tools effectively as references, without relying on them too much
- Chose clean, maintainable architecture and coding approaches to avoid technical debt
- Used AI to help review Pull Requests before merging into the main branch
- Set up automated checks, linting, and tests (unit + integration) in CI to reduce errors before deployment

## 3.2. What could have been better

- Team meetings were not scheduled well, causing inconvenience
- The business logic was quite complex, requiring multiple explanations for the whole team
- Design updates required matching changes in the UI code
- UML diagrams should follow the “diagram as code” approach to make editing and storing easier

## 3.3. What will we do differently

- Spread tasks more evenly across the weeks so the team has time to adjust instead of rushing everything at once
- Finalize design before coding to reduce changes later
- The project lead (Bình) should focus more on the project instead of handling too many unrelated tasks
- Different AI models have different strengths, so choose the right one for the right job (e.g., Gemini for planning and requirement analysis, Claude for coding tasks)
- Consider using a SCRUM style that leans more toward iterative development instead of incremental

## 3.4. Individual contributions and observations

- Trần Nguyễn Duy Minh:
  - Deliverables: Gantt chart, Communication Plan, Kick-off Meeting Minutes, Agile vs Waterfall (doc + slides), SCRUM meeting, Frontend code, Final Document
  - Assessment: Excellent. Always on time, never late on tasks, very responsible.

- Đào Duy Vinh:
  - Deliverables: Work Breakdown Structure, Quality Plan, Agile vs Waterfall, SCRUM meeting, Figma design
  - Assessment: Responsible, but personal matters affected coding progress.

- Nguyễn Thái Gia Nguyễn:
  - Deliverables: Project Charter, Human Resource Management document, SCRUM meeting, Backend code
  - Assessment: Very supportive and kept the whole team connected. Helped solve common issues. Suggested using Domain Driven Design, which made the code clearer and easier to maintain.

- Trần Nguyễn Thái Bình:
  - Deliverables: Stakeholders Register, Budget Management, Risk Register, SCRUM meeting, DevOps code
  - Assessment: Completed tasks well and helped make good technical decisions.

# 4. Personal Feedback

## 4.1. Trần Nguyễn Thái Bình

### 4.1.1. Knowledge

Em tham gia dự án lần này với vai trò là một Product Owner, Scrum Master, DevOps Engineer và Backend Developer, em đã có cơ hội mở rộng vốn hiểu biết cũng như kiến thức của bản thân mình không chỉ về mặt chuyên môn mà còn là về các kỹ năng mềm trong suốt dự án Electricilies. Em đã dành thời gian tìm hiểu về các khái niệm, các cộng nghệ về DevOps, như là cách xây dựng pipeline CI/CD, deploy ứng dụng trên Kubernetes,... . Em đã có được những kỹ năng cần thiết về monitoring và autoscaling. Em cũng nghiên cứu về các kiến trúc phần mềm trong việc thiết kế backend server, bên cạnh đó, em còn hiểu được cách làm sao đem lại những yếu tố thiết yếu để hỗ trợ nhóm và đảm bảo tính ổn định của hệ thống.

### 4.1.2. Skills

Kỹ năng về DevOps và backend của em đã được cải thiện một cách đáng kể. Em trở nên thành thạo trong việc cấu hình quy trình làm việc CI/CD, xử lý sự cố khi deploy và hỗ trợ các team khác release container. Em đã phát triển kỹ năng của một leader thực thụ và kỹ năng về tổ chức trong một team bằng cách quản lý các buổi họp Scrum hàng ngày, theo dõi tiến độ và điều phối công việc giữa các thành viên trong nhóm. Giải quyết vấn đề là một kỹ năng tối quan trọng và cần thiết, vì vậy em thường phải giải quyết các vấn đề cản trở và hỗ trợ người khác giải quyết các thách thức kỹ thuật cũng như về giao tiếp giữa các thành viên trong team.Qua đó, em cũng học được cách giao tiếp hiệu quả và triển khai tài liệu rõ ràng và mạch lạc.

### 4.1.3. Experience

Dự án Electricilies là một cơ hội giúp em tiếp cận gần hơnn những thách thức thực tế trong việc deploy phần mềm và phối hợp với các thành viên trong nhóm của mình. Em đã gặp phải những vấn đề như lỗi khi chạy CI/CD, trì hoãn trong việc release, deploy,... . Việc đảm nhận nhiều vai trò khác nhau đã giúp em học được cách cân bằng trách nhiệm và thời gian để đạt được hiệu quả tốt hơn. Em đã học được tầm quan trọng của hoàn thành các tài liệu liên quan đến dự án sớm để tiến đến triển khai cũng như code, theo dõi tiến độ làm việc của các thành viên trong nhóm. Những trải nghiệm này đã giúp em có thêm kinh nghiệm về quản lý cũng như.

### 4.1.4. Use of AI

Em đã sử dụng các công cụ AI để viết prompt và hoàn thành các tài liệu, tìm hiểu các kiến thức về mặt chuyên môn. AI giúp em làm việc hiệu quả hơn bằng cách cung cấp các mẫu, truy cập thông tin nhanh chóng hơn cũng như có thể gợi ý các giải pháp tối hơn cho dự án.Em đảm bảo đã xác thực và điều chỉnh các kết quả do AI tạo ra cho phù hợp với yêu cầu của dự án. Thông qua quá trình này, em đã học được cách tích hợp AI vào quy trình làm việc của mình như một công cụ hỗ trợ, nâng cao năng suất mà vẫn đảm bảo chất lượng và độ chính xác.

## 4.2. Nguyễn Thái Gia Nguyễn

### 4.2.1. Knowledge

Trong suốt dự án Electricilies, em đã tích lũy được kiến thức sâu sắc hơn về backend, đặc biệt là trong việc thiết kế và triển khai các RESTful API cho các module như sản phẩm, giỏ hàng và thanh toán. Em đã tìm hiểu về cơ chế xác thực và phân quyền thông qua Keycloak, đồng thời nghiên cứu các mô hình kiến trúc nâng cao như Domain Driven Design và Clean Architecture. Đây đều là những khái niệm mới đối với em, vì vậy em đã dành thêm nhiều thời gian để nghiên cứu bản chất, nguyên lý cũng như cách áp dụng chúng một cách hiệu quả vào hệ thống. Bên cạnh đó, em cũng mở rộng hiểu biết của mình về quản lý cơ sở dữ liệu, chiến lược caching và tích hợp các cổng thanh toán bên thứ ba như VNPay.

### 4.2.2. Skills

Kỹ năng của em đã cải thiện đáng kể trong quá trình tham gia dự án. Em đã trở nên thành thạo hơn trong việc tích hợp các thư viện bên ngoài, xử lý các giao dịch cơ sở dữ liệu phức tạp và tối ưu hiệu suất backend thông qua caching. Em cũng học được cách viết tài liệu API bằng Swagger, giúp việc phối hợp với nhóm frontend trở nên trơn tru hơn. Kỹ năng giao tiếp của em được cải thiện khi em thường xuyên cập nhật tiến độ và trao đổi về các vấn đề gặp phải với cả nhóm. Bên cạnh đó, kỹ năng quản lý thời gian và giải quyết vấn đề trở nên quan trọng khi em đảm nhận các nhiệm vụ khó và thích ứng với những thay đổi yêu cầu từ dự án.

### 4.2.3. Experience

Dự án mang đến rất nhiều thách thức đối với em, như làm việc với các thư viện có tài liệu hạn chế, tìm hiểu những mô hình kiến trúc phức tạp và chạy đua với tiến độ gấp rút. Em đã chịu áp lực trong việc đảm bảo hoàn thành tính năng đúng hạn và đôi khi phải refactor lại code để nâng cao chất lượng. Quá trình phối hợp với các thành viên trong nhóm giúp em nhận ra tầm quan trọng của giao tiếp rõ ràng và tinh thần làm việc nhóm. Em học được cách chủ động nhờ sự hỗ trợ khi cần thiết và hỗ trợ các bạn bằng cách chia sẻ tài liệu cũng như những hiểu biết kỹ thuật của mình. Những trải nghiệm này giúp em trưởng thành hơn cả về mặt chuyên môn lẫn khả năng làm việc nhóm.

### 4.2.4. Use of AI

Em đã sử dụng các công cụ AI chủ yếu cho việc tra cứu tài liệu kỹ thuật, tạo prompt cho các báo cáo và hỗ trợ kiểm thử API. AI giúp em tiết kiệm thời gian bằng cách cung cấp thông tin nhanh chóng và đưa ra các gợi ý hữu ích, đặc biệt khi em gặp khó khăn về kỹ thuật hoặc cần soạn thảo tài liệu. Tuy nhiên, em luôn xem xét và điều chỉnh lại nội dung do AI tạo ra để đảm bảo độ chính xác và phù hợp với yêu cầu của dự án. Thông qua quá trình làm việc, em nhận thấy AI là một công cụ hỗ trợ đắc lực, nhưng sự đánh giá và tinh chỉnh của con người vẫn là điều cần thiết để đảm bảo chất lượng cao nhất.

## 4.3. Trần Nguyễn Duy Minh

Trước đây, với việc chỉ được tiếp xúc với các dự án có quy mô nhỏ và phạm vi chỉ vỏn vẹn trong môn học, ngành học, em chưa có cơ hội trải nghiệm, làm quen với quy trình quản lý dự án trong thực tế. Trong quá trình tham gia học tập và hoạt động trong lớp SE358, em đã được mở rộng kiến thức, có một cái nhìn tổng quát hơn về cách một dự án được quản lý chặt chẽ, chỉnh chu.

Buổi đầu tiên, khi bước vào môn học với một cái nhìn còn mơ hồ về lĩnh vực này, em rất bất ngờ về lượng kiến thức khổng lồ cũng như bộ tài liệu đồ sộ trong phạm vi quản lý dự án. Từ quy tắc vàng - 5 nhóm quy trình, 10 lĩnh vực kiến thức, 49 quy trình - đến cách các lĩnh vực quản trị được thực hiện chi tiết trong một dự án. Trong quá trình học, dù xuất hiện một vài khó khăn trong việc tiếp thu vì chưa từng được làm quen với các quy trình này trước đây, nhưng em cũng đã chủ động kết hợp việc liên lạc với giảng viên và tra cứu qua Internet để vượt qua những khó khăn gặp phải. Bên cạnh đó, tài liệu hướng dẫn thực hành cũng chi tiết, phù hợp làm nền tảng để chúng em dựa vào đó thực hiện đồ án. Làm việc nhóm trong môn học này cũng đòi hỏi sự hợp tác chặt chẽ hơn các môn học cơ sở ngành khác. Mặc dù được mỗi người trong nhóm được phân công mỗi tài liệu khác nhau (ví dụ: bạn Bình làm Budget Plan, Nguyễn làm Resource Plan, Vinh làm Quality và em làm Communication), tuy nhiên các tài liệu đòi hỏi phải được kiểm tra chéo với nhau thường xuyên bởi các thành viên khác. Lý do là vì nội dung trong các bộ tài liệu phải được thống nhất, hợp logic và liên kết chặt chẽ với nhau. Do vậy, em luôn chủ động liên lạc trong nhóm mỗi khi có vấn đề hoặc mâu thuẫn cần phải làm rõ, giải quyết. Nhóm cũng chủ động tổ chức các cuộc họp thường xuyên nhằm thảo luận và đi đến một giải pháp chung cho các vấn đề trên. Ngoài ra, nhóm còn tìm hiểu và sử dụng bộ công cụ của Atlassian để quá trình làm việc được quản lý chặt chẽ và đơn giản hóa. Cụ thể, Atlassian Jira đã giúp em trong việc quản lý công việc và tiến độ thực hiện với các task và deadline được vạch ra rõ ràng, Atlassian Confluence là một công cụ quản lý tài liệu khá tốt và cũng giúp tăng cường khả năng hợp tác giữa các thành viên. Trong giai đoạn trải nghiệm Agile, em đã gặp phải một vài vấn đề trong việc làm quen do các dự án trước đây có quy mô nhỏ, chủ yếu sử dụng mô hình Waterfall nên chưa có kinh nghiệm với Agile. Giai đoạn này cũng đòi hỏi các thành viên trong nhóm nâng cao khả năng hợp tác thông qua Mini-Sprint và Scrum meeting. Nhìn chung, quá trình trải nghiệm Agile có hiệu quả tốt và em cũng đã được tìm hiểu về một mô hình phát triển dự án mới, thông dụng hiện hay, đồng thời cũng rút ra được sự khác nhau giữa Agile và Waterfall truyền thống để có cái nhìn đa chiều hơn về cả hai mô hình.

Trải nghiệm làm việc nhóm của em cũng khá thành công. Ban đầu phần giao tiếp còn khó khăn vì các thành viên còn tương đối rụt rè, tuy nhiên sau một thời gian làm quen thì cả nhóm đã có biểu hiện cởi mở hơn và khả năng giao tiếp cũng đã cải thiện ít nhiều. Các thành viên đều chủ động liên hệ khi gặp khó khăn và thảo luận với nhau đề tìm ra giải pháp. Dù vậy, trong quá trình thực hiện đồ án, các thành viên vẫn còn nhiều trường hợp trễ deadline khiến công việc bị delay, nhưng vấn đề này cũng càng ngày càng được khắc phục. Nhóm có điểm chung là ham học hỏi, đều tìm hiểu và tận dụng các công cụ nêu trên để đơn giản hóa quá trình làm việc. Các mâu thuẫn trong nhóm cũng được đi đến một giải pháp chung thông qua thảo luận hay các cuộc họp ngắn. Nhìn chung, dù còn một vài hạn chế nhưng em đã hoàn thành khá tốt vai trò làm việc nhóm.

Các công cụ AI cũng đã đóng góp một phần lớn trong quá trình thực hiện đồ án của em. Cụ thể, AI đã hỗ trợ bằng việc cung cấp một dàn ý chung và các giải thích chi tiết những phần trong các tài liệu. Kết hợp với việc tìm hiểu trên Internet, em đã có cái nhìn rõ hơn về cách triển khai các tài liệu này và cải thiện chúng để phù hợp với yêu cầu của môn học. Ngoài việc cấu trúc chung, AI còn giúp em đánh giá thông tin được đưa vào tài liệu. Nếu gặp một số đoạn diễn đạt quá mơ hồ, AI sẽ đưa ra các phản hồi mang tính xây dựng để em có thể điều chỉnh các đoạn này cho phù hợp.

Trong quá trình làm việc, AI đóng vai trò hỗ trợ hơn là thay thế kỹ năng ra quyết định. Các công cụ AI được biết đến rộng rãi nhờ khả năng xuất sắc trong việc đưa ra ý tưởng, cấu trúc tài liệu và đề xuất giải pháp hiệu quả cho nhiều vấn đề khác nhau. Em hoàn toàn đã có thể dựa vào AI để tạo ra tất cả tài liệu và thực hiện công việc thay cho bản thân mình, tuy nhiên, làm như vậy sẽ đi ngược lại hoàn toàn với mục đích học tập ngay từ ban đầu, và đồng thời cũng ngăn cản em trong việc phát triển các kỹ năng mà môn học này có thể đem lại. Thay vì chỉ copy paste các phản hồi thô của AI, em đã cẩn thận xây dựng prompt để thêm vào càng nhiều ngữ cảnh và ví dụ càng tốt. Sau đó, em kiểm tra tính phù hợp của phản hồi với bối cảnh của dự án và hướng giải quyết vấn đề của em hay không. Trong một số trường hợp, em phải viết lại gần như toàn bộ các phần để phù hợp với ý tưởng của mình, tuy nhiên, phản hồi ban đầu vẫn mở ra nhiều khía cạnh mới của vấn đề và giúp em có một hướng suy nghĩ thích hợp. Khả năng suy nghĩ tuyệt vời của AI không phải là để chúng ta lợi dụng. Vẫn còn phần lớn công việc mà AI không thể làm được, và các công việc đó đòi hỏi khả năng tư duy, phán đoán của riêng con người.

Nhìn chung, môn học đã cho em nền tảng vững chắc trong lĩnh vực quản lý dự án. Với kiến thức, trải nghiệm đã được học, chắc chắn sau này em sẽ không còn bỡ ngỡ khi tiếp xúc với một dự án thực tế khi bước trên con đường sự nghiệp của bản thân nữa. Em rất biết ơn với khối lượng kiến thức mà môn học này đã mang lại, cũng như sự tận tình của giảng viên trong việc hỗ trợ, giúp đỡ em thực hiện đồ án. Em sẽ tiếp tục áp dụng kiến thức mình đã học được vào những môn học cao hơn, và vào quá trình hoạt động trong các dự án lớn trong tương lai xa.
