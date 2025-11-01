# Báo cáo giai đoạn A

Lớp: SE358.Q12
Giảng viên: Lê Văn Tuấn

Thành viên:

Nguyễn Thái Gia Nguyễn - 23521049
Đào Duy Vinh - 23521787
Trần Nguyễn Duy Minh - 23520956
Trần Nguyễn Thái Bình - 23520161

# 1. Project Charter

## 1.1 Project Details

|                         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Project Name**        | eCommerce Website for Electronic Products                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Project Description** | This project aims to design, develop, and launch a fully functional eCommerce website for selling electronic products such as laptops, smartphones, tablets, accessories, and home appliances. The platform will offer an intuitive user interface, secure payment options, inventory management, and customer support features. The website will serve both retail and wholesale customers, providing a seamless shopping experience on desktop and mobile devices. |
| **Project Goals**       | **Develop a user-friendly website** that enables customers to easily browse, search, and purchase electronic products.                                                                                                                                                                                                                                                                                                                                               |
| **Project Team**        | - **Drivers:** Trần Nguyễn Thái Bình, Nguyễn Thái Gia Nguyễn<br>- **Approvers:** Trần Nguyễn Thái Bình, Nguyễn Thái Gia Nguyễn<br>- **Contributors:** buggilies team (Nguyễn Thái Gia Nguyễn, Trần Nguyễn Thái Bình, Trần Nguyễn Duy Minh, Đào Duy Vinh)                                                                                                                                                                                                             |
| **Budget**              | Estimated budget: **$50,000 – $70,000 USD** <br>This includes design, development, testing, hosting, marketing, and initial maintenance costs.                                                                                                                                                                                                                                                                                                                       |

## 1.2. Project Milestones & Schedule

FIXME: ADD TIMELINE DOOOOOOOOOOOOOOOOOO

## 1.3. SMART objectives

|     | **Goals**                                            | SHow is it **specific?**                                                               | MHow is **measurable?**                                                      | AHow is it **attainable?**                                            | RHow is it **relevant?**                                  | THow is it **time-based?**                          |
| --- | ---------------------------------------------------- | -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------- |
| 1   | Complete Product Management System                   | Develop an admin and seller product management page.                                   | Support adding, editing, deleting, and displaying at least **500 products**. | Implemented using Postgres, keycloak and a dedicated admin interface. | Core functionality of the e-commerce website.             | To be completed by **Week 6**.                      |
| 2   | Develop Shopping Cart and Checkout Features          | Enable users to add products to the cart, view total price, and place orders.          | Successfully process orders with **at least 5 different products**.          | Built through API integration between frontend and backend.           | Essential for completing the online shopping process.     | To be finished and tested by **Week 9**.            |
| 3   | Implement User Registration and Login System         | Create a secure authentication system using JWT or session management.                 | 100% successful login and registration during demo testing.                  | Use bcrypt for password hashing and middleware for access control.    | Fundamental to user management in an e-commerce platform. | Completed by **Week 5**.                            |
| 4   | Add Product Search and Filtering Functions           | Allow users to search and filter products by name, category, or price.                 | Query response time under **2 seconds**.                                     | Implemented through optimized database queries and pagination.        | Improves user experience and navigation efficiency.       | Ready by **Week 8**.                                |
| 5   | Build Order Management Module                        | Enable admins to view, update, and manage order statuses.                              | Capable of processing and displaying **at least 100 test orders**.           | Based on previously designed database models.                         | Key part of the order fulfillment workflow.               | Completed by **Week 10**.                           |
| 6   | Design an Optimized Database Structure               | Create an ERD and establish relationships among user, product, order, and cart tables. | Ensure no redundant data and maintain referential integrity.                 | Using PostgreSQL.                                                     | Forms the technical foundation of the project.            | Completed and reviewed by **Week 4**.               |
| 7   | Ensure Data and User Security                        | Encrypt passwords, implement authentication, and secure all APIs.                      | Achieve **zero major security vulnerabilities** in internal testing.         | Apply JWT, HTTPS (mock), and CSRF protection.                         | Protects customer data and builds trust.                  | Security testing finished by **Week 11**.           |
| 8   | Optimize System Performance                          | Improve loading speed and API response times.                                          | Main pages load within **3 seconds** on standard devices.                    | Through caching, compression, and lazy loading.                       | Enhances user satisfaction and usability.                 | Optimization completed by **Week 11–12**.           |
| 9   | Maintain Clear Task Assignment and Progress Tracking | Each team member has defined responsibilities (frontend, backend, or UI).              | **100% of tasks** updated on the project management tool (Git).              | Conduct bi-weekly meetings and progress updates.                      | Ensures accountability and project control.               | Monitored weekly throughout the **entire project**. |
| 10  | Deliver Final Demo and Comprehensive Report          | Produce a fully functional demo and detailed project report.                           | Submitted on time and meets instructor evaluation criteria.                  | Based on completed deliverables and testing.                          | Represents the final goal of the project.                 | Completed by **Week 12**.                           |

# 2. Stakeholder Register

| **Stakeholder Name** | **Role**         | **Category** | **Influence** | **Interest** | **Expectation**                                         | **Communication**  | **Communication frequency** | **Contact**                                |
| -------------------- | ---------------- | ------------ | ------------- | ------------ | ------------------------------------------------------- | ------------------ | --------------------------- | ------------------------------------------ |
| Project Sponsor      | Executive        | INTERNAL     | STRONG        | STRONG       | High ROI, on-time/on-budget delivery, market success.   | Meetings, Reports  | Weekly/Monthly              | TBD                                        |
| Project Manager      | Management       | INTERNAL     | STRONG        | STRONG       | Successful project delivery, meeting all requirements.  | Meetings, Email    | Daily                       | `kevinnitro@duck.com`                      |
| Development Team     | Technical Staff  | INTERNAL     | NEUTRAL       | STRONG       | Clear requirements, stable development environment.     | Stand-ups, Chat    | Daily                       | `buggilies@googlegroups.com`               |
| Admin                | System Operator  | INTERNAL     | NEUTRAL       | STRONG       | A stable, secure, and monitorable system.               | Reports, Alerts    | As Needed                   | `admin@electricilies.com`                  |
| Staff                | Business User    | INTERNAL     | NEUTRAL       | STRONG       | Efficient tools to manage products, users, and reviews. | Training, Meetings | Weekly                      | `staff@electricilies.com`                  |
| Customers            | End User         | EXTERNAL     | WEAK          | STRONG       | A functional, easy-to-use website to buy products.      | Website, Email     | As Needed                   | N/A                                        |
| Suppliers            | Partner          | EXTERNAL     | NEUTRAL       | NEUTRAL      | A reliable platform for selling their products.         | Email, Portal      | Monthly                     | `supplier1@mail.com`, `supplier2@mail.com` |
| Payment Gateway      | Service Provider | EXTERNAL     | WEAK          | WEAK         | Seamless integration and transaction processing.        | API Docs, Email    | As Needed                   | `hotrovnpay@vnpay.vn`                      |

# 3. Work Breakdown Structure - WBS

FIXME: Dán hình dô

# 4. Gantt charts

FIXME: Dán hình vô

# 5. Retrospective

## 5.1. What went well

- Early project identification, reasonable division of tasks
- Team members cooperated well and were responsible
- Chose Atlassian Jira to divide and track tasks
- Selected good templates (from Confluence, online) for use

## 5.2. What could have been better

- Unified platform and workspace (Atlassian Confluence, Google Docs, platforms supporting diagram drawing)
- Made better use of Atlassian Confluence apps (extensions) to maximize work efficiency

## 5.3. What will we do differently

- Organize meetings more frequently to address team members' questions
- Use Confluence for documentation to make it easier to consolidate information

# 6. Appendix

## 6.1. Prompts

Below are prompts for corresponding sections

### 6.1.1. Project Charter

```markdown
Please use the following template to write the structure for my Project Charter, based on the PMI project charter framework and the Atlassian Project Charter Template from this link: https://www.atlassian.com/software/confluence/templates/project-charter

1. First, propose the ideal structure for my Project Charter, combining PMI’s standard sections (such as Purpose, Objectives, Scope, Deliverables, Risks, Stakeholders, etc.) with the sections from the Atlassian template.
2. Then, suggest sample content or guiding questions for each section — enough to help me fill in details for my own project later.
3. After that, create a SMART Objectives Table in Markdown format, using the following structure (leave the table empty so I can fill it in myself):

| Goals | How is it Specific? | How is it Measurable? | How is it Attainable? | How is it Relevant? | How is it Time-Based? |
| ----- | ------------------- | --------------------- | --------------------- | ------------------- | --------------------- |
| 1     |                     |                       |                       |                     |                       |
|       |                     |                       |                       |                     |                       |
```

### 6.1.2. Stakeholders Register

````markdown
my project is **Electricilies - Website for Selling Electronic Products**, can you list out to fill in the stakeholder register table?

Here is the template

```markdown
| Stakeholder Name | Role | Category | Influence | Interest | Expectation | Communication | Communication frequency | Contact |
| ---------------- | ---- | -------- | --------- | -------- | ----------- | ------------- | ----------------------- | ------- |
|                  |      | INTERNAL | NEUTRAL   | STRONG   |             |               | Daily                   |         |
|                  |      | EXTERNAL | STRONG    | NEUTRAL  |             |               | Weekly                  |         |
|                  |      |          | WEAK      | WEAK     |             |               |                         |         |
```

category, influence, interest is only have those fields, Communication frequency is variety
````

- After prompting, the AI generated a list of stakeholder groups and their respective fields. We supplemented the list of missing stakeholders and identified possible contacts of some stakeholders.

## 6.2. Self reports

### 6.2.1 Docker

Phân tích dự án Docker - Nguyễn Thái Gia Nguyễn

#### 6.2.1.1. Giới thiệu dự án

Docker là một nền tảng mã nguồn mở ra mắt vào năm 2013, được thiết kế để đơn giản hóa quá trình xây dựng, triển khai và chạy ứng dụng trong môi trường **container**. Dự án bắt nguồn từ công ty dotCloud (sau này đổi tên thành Docker, Inc.), do **Solomon Hykes** sáng lập. Ý tưởng của Docker là cung cấp một cách đóng gói ứng dụng cùng toàn bộ môi trường của nó (thư viện, cấu hình, phụ thuộc) vào một container nhẹ, có thể chạy đồng nhất trên mọi máy chủ.

Docker nhanh chóng trở thành một cuộc cách mạng trong lĩnh vực phát triển và vận hành phần mềm (DevOps), thay thế cho cách tiếp cận truyền thống bằng **máy ảo (VM)**. Từ đó, Docker trở thành nền tảng cốt lõi trong xu hướng **cloud-native** và **microservices**.

#### 6.2.1.2. Phân tích các yếu tố

##### 6.2.1.2.1. Phạm vi (Scope)

- **Ban đầu**:
  - Cung cấp công cụ đóng gói ứng dụng thành container.
  - Đảm bảo ứng dụng chạy nhất quán từ máy dev đến production.
- **Phát triển**:
  - Tích hợp Docker Hub (kho chia sẻ container image).
  - Docker Compose cho multi-container apps.
  - Docker Swarm cho orchestration.
  - Hỗ trợ CI/CD, cloud, và container registry.
- **Phạm vi mở rộng**:
  - Trở thành nền tảng toàn cầu cho containerization.
  - Nền tảng trung tâm trong hệ sinh thái **Kubernetes** và cloud.

##### 6.2.1.2.2. Tiến độ (Schedule)

- 2008–2012: Ý tưởng ban đầu từ dự án **dotCloud**.
- 2013: Docker ra mắt công khai tại PyCon, viết bằng Python ban đầu.
- 2014: Chuyển codebase sang **Go** → hiệu năng tốt hơn.
- 2015: Docker Inc. ra mắt Docker Swarm, Compose.
- 2017 trở đi: Kubernetes dần thống trị orchestration, Docker tập trung vào Docker Desktop, Hub.
- Hiện tại: Docker vẫn là công cụ chính cho dev, còn orchestration do Kubernetes dẫn đầu.

**Tiến độ thực tế**: Docker phát triển bùng nổ chỉ sau 1–2 năm, trở thành tiêu chuẩn công nghiệp, vượt xa kỳ vọng ban đầu của dotCloud.

##### 6.2.1.2.3. Chi phí (Cost)

- **Chi phí ban đầu**: Do dotCloud tự đầu tư, sau đó nhận vốn từ Y Combinator và các quỹ VC(Venture Capital Fund).
- **Chi phí vận hành**:  
  • Phát triển phần mềm mã nguồn mở.  
  • Duy trì Docker Hub, Docker Desktop.
- **Doanh thu**:  
  • Bản thương mại (Docker Enterprise, sau này bán cho Mirantis).  
  • Docker Desktop trả phí cho doanh nghiệp lớn.
- **Kết luận**: Docker Inc. gặp khó khăn về mô hình kinh doanh, nhưng công nghệ Docker trở thành chuẩn chung, tạo tiền đề cho nhiều công ty khác.

##### 6.2.1.2.4. Chất lượng (Quality)

- **Người dùng**: Developer trải nghiệm tốt, “build once, run anywhere”.
- **Công nghệ**: Container nhẹ, nhanh, hiệu quả hơn VM.
- **Hệ sinh thái**: Kho image khổng lồ trên Docker Hub.
- **Thách thức**: Quản lý bảo mật image, chuẩn hóa orchestration.

##### 6.2.1.2.5. Nguồn lực (Resources)

- **Nhân sự**: Ban đầu nhỏ (Solomon Hykes + đội dotCloud), sau mở rộng với cộng đồng open-source toàn cầu.
- **Công nghệ**: Chuyển từ Python sang Go để đạt hiệu năng cao.
- **Tài chính**: Gọi vốn từ các quỹ đầu tư mạo hiểm.
- **Cộng đồng**: Cộng đồng open-source là nguồn lực mạnh mẽ nhất của Docker.

##### 6.2.1.2.6. Rủi ro (Risks)

- **Pháp lý**: Vấn đề bản quyền image, bảo mật container.
- **Cạnh tranh**: Podman, rkt (CoreOS, sau này ngừng), và đặc biệt là **Kubernetes** (Google).
- **Chiến lược kinh doanh**: Docker Inc. từng thất bại trong việc monetization, buộc phải bán mảng enterprise cho Mirantis.
- **Hạ tầng**: Áp lực duy trì Docker Hub.
- **Uy tín**: Mất vị thế dẫn đầu orchestration về tay Kubernetes.

#### 6.2.1.3. Bài học rút ra

1. **Giải quyết nhu cầu thực tế**: Docker thành công vì đơn giản hóa việc triển khai ứng dụng.
2. **Cộng đồng là chìa khóa**: Sự bùng nổ của Docker nhờ cộng đồng open-source.
3. **Chọn công nghệ phù hợp**: Việc chuyển từ Python sang Go giúp tăng hiệu năng đáng kể.
4. **Kinh doanh khó hơn công nghệ**: Dù công nghệ thành công, Docker Inc. gặp nhiều khó khăn trong mô hình doanh thu.
5. **Tầm quan trọng của hệ sinh thái**: Docker đặt nền móng cho Kubernetes và cloud-native, chứng minh rằng giá trị lớn nhất không chỉ là sản phẩm mà là cả hệ sinh thái.

Tóm lại: Docker khởi đầu như một ý tưởng đơn giản từ dotCloud, nhưng đã trở thành một cuộc cách mạng trong thế giới phần mềm. Tuy công ty Docker Inc. không giữ được vị thế thống trị, nhưng **Docker (container)** đã thay đổi hoàn toàn cách ngành công nghệ triển khai và vận hành ứng dụng.

### 6.2.2. OSU!Lazer

Phân tích dự án trò chơi âm nhạc trực tuyến osu!lazer - Đào Duy Vinh

#### 6.2.2.1 Bối cảnh

- **osu!** (hay **osu!stable**) là tựa game âm nhạc được ra mắt trên nền tảng PC vào năm 2007 bởi Dean "peppy" Herbert dựa trên trò chơi cùng tên (Osu! Tatakae! Ouendan!) được phát hành trên Nintendo DS vào năm 2005. Dự án gây được tiếng vang lớn nhờ gameplay dễ gây nghiện nhưng cũng đầy thử thách, nhiều chế độ chơi khác nhau cũng như một cộng đồng lớn mạnh. Theo thống kê trên trang chủ của tựa game ([https://osu.ppy.sh](https://osu.ppy.sh)) vào 16/10/2025, ở Việt Nam có khoảng 57,022 người chơi hoạt động thường xuyên với tựa game này.
- Tuy nhiên, do được thiết kế và lập trình trên nền tảng công nghệ cũ, tuy vẫn đang hoạt động cho đến thời điểm hiện tại nhưng trò chơi vẫn mắc phải một số điểm bất cập như việc tình trạng giật lag xảy ra thường xuyên, mất kết nối đến máy chủ cũng như chế độ nhiều người chơi hoạt động thiếu ổn định. Song song với đó, tựa game cũng bị giới hạn về công nghệ và khả năng mở rộng. Để khắc phục những điểm yếu kể trên cũng như giúp tựa game phù hợp hơn với thời đại, vào năm 2017, peppy đã ra mắt dự án **osu!lazer** với nhiều hứa hẹn đến từ chính nhà phát triển. Tuy nhiên sau 8 năm xây dựng, đến hiện tại tựa game vẫn chưa thể đưa được cho cộng đồng một phiên bản trò chơi tương xứng với kì vọng.
- Dự án được phát hành dưới dạng **mã nguồn mở trên GitHub**, được phát triển liên tục dưới sự đóng góp của cộng đồng.

#### 6.2.2.2. Phân tích các yếu tố

##### 6.2.2.2.1. Phạm vi (Scope)

- Mục tiêu xuyên suốt của osu!lazer là **viết lại toàn bộ kiến trúc của tựa game cũ** bằng những công nghệ hiện đại hơn (.NET 6, cross-platform, UI framework riêng,...) nhằm mục đích tối ưu hóa hiệu năng cũng như khả năng mở rộng và đa nền tảng (Windows, Linux, MacOS, Android và IOS). Đồng thời, trò chơi cũng **giữ gìn gameplay cốt lõi** đi kèm **với nhiều tính năng mới** như chế độ chơi trực tuyến được mở rộng, thêm các mod mới để thay đổi gameplay, khả năng tự tạo các chế độ chơi mới thông qua ruleset API,...
- Tuy phạm vi lớn là vậy, dự án vẫn có **lộ trình rõ ràng và công khai** trên GitHub, được chia thành các **cột mốc (milestone)** như framework, engine, UI, gameplay và hệ thống trực tuyến, thể hiện khả năng quản lý phạm vi hiệu quả.

##### 6.2.2.2.2. Tiến độ (Schedule)

- Dự án được khởi động từ **năm 2017**, và vẫn đang trong quá trình phát triển sau **8 năm** ròng rã. Tuy vậy, người chơi vẫn được tiếp cận với tựa game thông qua các bản cập nhật nhỏ hàng tuần được phát hành thông qua GitHub Actions.
- Dự án được phát triển mã nguồn mở, mọi tính năng đều được thiết kế, thử nghiệm và phải hồi **công khai** trên GitHub, khiến tiến độ chậm hơn nhưng được **chất lượng và minh bạch.**
- Phần lớn thời gian phát triển cũng được phân bổ cho việc chuẩn hóa gameplay, chuyển đổi dữ liệu cũ, và tối ưu hóa khả năng hoạt động đa nền tảng (Windows, macOS, Linux, Android, iOS).
- Bên cạnh đó, đội ngũ phát triển osu!lazer cũng có phần khiêm tốn về mặt số lượng nhân sự, phần nào đó cũng ảnh hưởng đến quá trình hoàn thiện trò chơi.

##### 6.2.2.2.3. Chi phí (Cost)

- osu!lazer -- cũng như phiên bản trước đó -- là dự án **mã nguồn mở và phi lợi nhuận**. Tất cả những chi phí liên quan đến nhân sự, duy trì trò chơi đều đến từ đóng góp tự nguyện thông qua osu! supporter (một hình thức đăng kí tính năng có trả phí) và các khoản ủng hộ khác nhau. Những người chơi có trình độ tin học cao hơn có thể đóng góp vào dự án thông qua việc trở thành các Developer Volunteer -- trực tiếp tham gia vào quá trình phát triển trò chơi.
- Nhờ vào đó, dự án **không phải chịu áp lực lớn về tài chính** như các dự án game thương mại khác -- hay nói cách khác, dự án được tự do để toàn lực dốc sức vào chính chất lượng của trò chơi thay vì phải chịu sự áp lực hay giám sát từ các nhà đầu tư.
- Tuy vậy, việc phụ thuộc lớn vào tinh thần đóng góp tự nguyện của trò chơi cũng mang lại một số **hạn chế** cho chính bản thân dự án như ảnh hưởng đến tiến độ phát triển, gây phân tán nguồn lực kĩ thuật hay rủi ro về việc duy trì ổn định lâu dài.
- Đến hiện tại, mô hình vẫn chứng minh được tính bền vững và sức ảnh hưởng của osu!, trở thành một ví dụ điển hình về **cách một dự án cộng đồng có thể phát triển quy mô toàn cầu mà không cần mô hình thương mại truyền thống**.

##### 6.2.2.2.4. Chất lượng (Quality)

- Dự án làm lại của tựa game cũ có **một số điểm cải thiện đáng kể**: Giao diện trò chơi đẹp, thân thiện và dễ nhìn hơn so với bản cũ; các tính năng chơi được mở rộng và khả năng tùy biến cao; hỗ trợ đa nền tảng.
- Tuy vậy, phần lớn người chơi **vẫn chọn ở lại với phiên bản stable của trò chơi**, cho rằng dự án mới vẫn đang quá thiếu hoàn thiện. Điều này có thể thấy ở rất nhiều điểm bất cập của lazer: Thiếu đi một số tính năng quan trọng, đặc biệt là trình biên tập map chơi; yêu cầu cấu hình cao hơn so với tựa game gốc; các vấn đề về tương thích với các map chơi/skin ở phiên bản cũ. Đặc biệt, dù được tối ưu về mặt công nghệ, tựa game mới vẫn thiếu đi độ ổn định; các yếu tố về giật lag vẫn hay xảy ra, một số tính năng cũ ở gameplay hoạt động thiếu nhất quán và vấn đề nghiêm trọng nhất là **độ trễ đầu vào (input latency)** -- yếu tố ảnh hưởng trực tiếp đến độ chính xác trong một tựa game dựa vào nhịp điệu âm nhạc.
- Với các yếu tố trên, có thể nói dự án lazer vẫn chưa thể thay thế hoàn toàn phiên bản cũ, người chơi -- đặc biệt là các streamer chuyên nghiệp và người chơi thi đấu -- vẫn trung thành hơn với phiên bản cũ, vốn mang lại cảm giác chơi ổn định, chính xác và đáng tin cậy hơn.

##### 6.2.2.2.5. Rủi ro (Risks)

- Mô hình phát triển mở và phi lợi nhuận khiến osu!lazer **phụ thuộc mạnh vào tinh thần đóng góp tự nguyện của cộng đồng**. Nếu sự quan tâm giảm sút, tiến độ có thể bị chậm lại hoặc gián đoạn. Bên cạnh đó, sự phân tán về nhân lực và trình độ kỹ thuật giữa các cộng tác viên cũng dẫn đến khó khăn trong việc duy trì chất lượng mã nguồn thống nhất, dễ phát sinh lỗi hoặc xung đột phần mềm.
- Do dự án phát triển song song với phiên bản stable, nguy cơ **chia rẽ cộng đồng người chơi** là hiện hữu: một bộ phận ủng hộ lazer, trong khi phần lớn vẫn trung thành với phiên bản cũ vì tính ổn định. Điều này xuất phát từ việc lazer vẫn đang trong giai đoạn hoàn thiện làm cho rủi ro về trải nghiệm người dùng khá cao, điều này có thể ảnh hưởng tiêu cực đến uy tín của trò chơi nếu không được khắc phục triệt để.
- Về lâu dài, nếu không có chiến lược chuyển đổi người dùng hoặc nguồn lực ổn định hơn, dự án có thể **rơi vào tình trạng "phát triển kéo dài"** mà không đạt đến giai đoạn phát hành chính thức.

#### 6.2.2.3. Bài học rút ra

- Dự án osu!lazer vốn có rất nhiều tiềm năng để thay thế người đàn anh của mình để trở thành phiên bản kế nhiệm xứng đáng của trò chơi nổi tiếng, tuy vậy tựa game mới vẫn để lại nhiều điều tiếc nuối sau 8 năm dài đã và đang phát triển. Từ đó, ta có thể rút ra được nhiều bài học sâu sắc về quản lý dự án và phát triển phần mềm quy mô lớn.
- Trước hết, việc **xác định phạm vi và lộ trình hợp lý** là yếu tố then chốt. Dự án lazer đặt mục tiêu quá rộng -- viết lại toàn bộ trò chơi, chuyển sang công nghệ mới, hỗ trợ đa nền tảng và mở rộng hệ thống gameplay -- dẫn đến tiến độ kéo dài nhiều năm. Điều này cho thấy tầm quan trọng của việc **phân chia mục tiêu thành từng giai đoạn rõ ràng**, có thể kiểm soát và đánh giá được.
- Bên cạnh đó, **công nghệ hiện đại không đảm bảo ngay lập tức mang lại trải nghiệm tốt hơn**. Dù osu!lazer áp dụng .NET 6 và kiến trúc tiên tiến, phần lớn người chơi vẫn trung thành với phiên bản stable vì sự ổn định, quen thuộc và độ chính xác cao. Từ đó có thể thấy, trong phát triển sản phẩm, **sự đổi mới kỹ thuật cần đi đôi với việc thấu hiểu nhu cầu và thói quen của người dùng**.
- Dự án cũng minh chứng rằng **mô hình mã nguồn mở** tuy mang lại tính tự do và minh bạch, nhưng đòi hỏi **năng lực điều phối và tổ chức cộng đồng hiệu quả**. Khi nguồn lực đến từ đóng góp tự nguyện, việc duy trì tiến độ, kiểm thử và chất lượng phần mềm trở nên khó khăn hơn đáng kể.
- Cuối cùng, **osu!lazer nhấn mạnh tầm quan trọng của tính ổn định và hiệu năng** trong các trò chơi nhịp điệu. Chỉ cần sai lệch nhỏ về độ trễ đầu vào cũng có thể ảnh hưởng lớn đến trải nghiệm người chơi. Một sản phẩm bền vững không chỉ dựa vào công nghệ mới, mà còn vào **sự kiên trì, lắng nghe phản hồi và tầm nhìn dài hạn của đội ngũ phát triển**.

### 6.2.3. Crse

Phân tích dự án Crse - Trần Nguyễn Duy Minh

Trước đây, các dự án phần mềm em thực hiện đều xuất phát từ sở thích cá nhân nên không có kiến trúc, quy trình hay tài liệu đầy đủ. Nhằm tìm hiểu và làm quen với quy trình thực hiện một dự án phần mềm, em đã chọn đề tài liên quan đến Hệ thống Website Quản lý lớp học Online (từ đây sẽ gọi là Crse) để thực hiện trong dự án môn học Nhập môn Công nghệ Phần mềm. Dự án có quy mô nhỏ, với mục tiêu là tạo ra một nền tảng giúp học viên và giảng viên có thể trao đổi hoạt động học tập trực tuyến thay vì Messenger hay Zalo. Nhóm cũng tận dụng thời gian thực hiện dự án để làm quen với các khái niệm chuyên ngành và các công cụ hỗ trợ có liên quan.

Crse chỉ hỗ trợ tiếng Việt và nhắm đến đối tượng người dùng là học sinh, giáo viên và các cơ sở giáo dục trong nước. Nhóm có tham khảo các hệ thống hiện hành tương tự như Classroom hay Moodle và thiết kế hệ thống với các chức năng chính như xác thực và phân quyền người dùng, quản lý môn học, đăng tải tài liệu, nộp bài tập, tạo và làm bài thi, và forum thảo luận cho mỗi lớp học. Dù vậy do nguồn lực và thời gian có hạn nên hệ thống chỉ triển khai ở phạm vi một lớp học và chưa có các chức năng nâng cao như chấm điểm tự động.

Lộ trình thực hiện dự án song song với nội dung của bài giảng trên lớp, cụ thể:

- **Tuần 1-2:** Thu thập yêu cầu, thiết kế form khảo sát về thói quen học tập online ở nhà, trao đổi tài liệu qua các kênh liên lạc hiện hành, các bất cập của các hệ thống đó.
- **Tuần 3-4:** Nhóm bắt đầu mô hình hóa yêu cầu, làm ERD, làm Function List, User Story, thiết kế sơ đồ Use-case và đặc tả.
- **Tuần 5-6:** Vẽ các sơ đồ Sequence, Activity cho các Use-case. Vẽ sơ đồ trạng thái, sơ đồ miền cho dự án.
- **Tuần 7:** Lên thiết kế cho giao diện và các UI Components.
- **Tuần 8-10:** Lập trình Front-end và Back-end.
- **Tuần 11-12:** Kiểm thử hệ thống và sửa các bug được phát hiện.
- **Tuần 13:** Hoàn thiện báo cáo đồ án.

Thực tế, dự án gặp nhiều khó khăn để theo kịp lộ trình đã đề ra do các thành viên trong nhóm đều chưa thành thạo trong nhiều giai đoạn của quy trình, đặc biệt là phần vẽ Diagram. Nhóm phải liên tục trao đổi với giảng viên để được hỗ trợ. Ngoài ra, các thành viên trong team Backend phải dành thời gian để học JavaScript và tìm hiểu về NodeJS và ExpressJS. Nhóm cũng phân vân trong việc lựa chọn hệ quản trị cơ sở dữ liệu thích hợp cho dự án. Tuy nhiên, các chức năng chính và giao diện của hệ thống vẫn được hoàn thành và triển khai trước ngày báo cáo môn học.

Do quy mô nhỏ nên dự án không tốn chi phí để phát triển, nhóm đã sử dụng Free Plan trên Vercel để host Front-end và Render để host Back-end. Tuy nhiên, vì chính sách miễn phí của Render nên mỗi lần gửi request, server phải cần khoảng 1 phút để khởi động. Bên cạnh đó, nhóm còn sử dụng các công cụ miễn phí như GitHub để lưu source code và Figma để thiết kế giao diện.

Sản phẩm đạt được vài ưu điểm nổi bật như giao diện thân thiện, dễ làm quen và sử dụng. Các chức năng cơ bản của hệ thống như xác thực và phân quyền, đăng tải file, nộp bài tập được hoàn thành và hoạt động như yêu cầu. Thời gian phản hồi request, thời gian truy xuất từ hệ cơ sở dữ liệu cũng đáp ứng yêu cầu dưới 1 giây. Tuy nhiên, hệ thống vẫn tồn tại nhiều hạn chế, ví dụ như một vài form chưa có xác thực dữ liệu nhập vào; hệ thống xác thực chỉ mới sử dụng Google OAuth chứ chưa có tùy chọn đăng nhập bằng tài khoản và mật khẩu; giao diện chưa được tối ưu cho điện thoại.

Nhóm thực hiện dự án gồm 3 thành viên, được phân công rõ ràng: 1 người thiết kế giao diện và lập trình Front-end sử dụng Figma, thư viện React và TailwindCSS, 2 người lập trình Back-end sử dụng ExpressJS và NodeJS, cả nhóm tham gia thiết kế cơ sở dữ liệu MySQL và viết tài liệu, báo cáo bằng LaTeX thông qua Overleaf. Các nguồn tài liệu học tập gồm w3schools, freeCodeCamp, Youtube,\... Mã nguồn của dự án được lưu trên GitHub. Vì kinh nghiệm còn hạn chế nên nhóm đều sử dụng các nền tảng quen thuộc và công nghệ đơn giản.

Trong quá trình phát triển, dự án đã gặp một số rủi ro. Đặc biệt nhất là rủi ro về bảo mật khi nhóm chưa có kinh nghiệm trong việc xử lý các lỗ hổng dữ liệu. Ngoài ra, do sử dụng Free Plan của Render nên hệ thống mang đến trải nghiệm người dùng không được tốt do server chỉ có thể chịu được lượng request thấp và cần thời gian để khởi động. Hệ thống còn có nguy cơ bị quá tải khi lượng người dùng truy cập đồng thời cao.

Dự án có thể được xem là thành công ở mức độ môn học do đã có sản phẩm và demo chạy được với các chức năng cơ bản. Bộ tài liệu của dự án cũng được hoàn thành theo chuẩn của môn học và được giảng viên chấp nhận. Tuy nhiên, nếu xét đến mục tiêu ban đầu nhóm đề ra thì dự án chưa được xem là thành công trọn vẹn. Các chức năng như chấm điểm tự động hay giao diện mobile vẫn chưa được hoàn thiện đúng lộ trình. Nguyên nhân chính là việc quản lý tiến độ chưa chặt chẽ, một số thành viên không đảm bảo được thời gian làm việc, còn delay deadline. Dù vậy, trong tương lai, hệ thống vẫn tiếp tục được phát triển thêm và sửa lỗi để hoàn thiện hơn.

Crse chính là dự án đầu tiên trong lĩnh vực phần mềm của nhóm, vì thế, nhóm đã tiếp cận được rất nhiều kiến thức mới cũng như rút ra được nhiều kinh nghiệm quý báu. Trước đây, chúng em đã nghĩ phát triển phần mềm chỉ đơn giản là code, tuy nhiên, trong thực tế việc code chỉ chiếm khoảng 30% trong quy trình phát triển. Trước hết, việc xác định phạm vi dự án cũng như phân tích yêu cầu đóng vai trò rất quan trọng vì chúng là nền tảng cho dự án, giảm thiểu các rủi ro trong các giai đoạn phía sau. Các rủi ro được sinh ra càng sâu trong quá trình phát triển sẽ dẫn đến thiệt hại càng lớn. Ngoài ra, nhóm đã có cơ hội làm quen với việc mô hình hóa yêu cầu qua các loại sơ đồ khác nhau. Bên cạnh đó, nhóm cũng cân nhắc sử dụng Jira cho các dự án sau nhằm quản lý tiến độ vì rõ ràng việc không kịp tiến độ là nhược điểm lớn nhất của dự án lần này. Tóm lại, đây đều là những bài học quý giá có thể áp dụng trong không chỉ các dự án sau này mà còn là môi trường làm việc trong tương lai.

### 6.2.4. Kubernetes

Phân tích dự án Kubernetes - Nguyễn Thái Gia Nguyễn

#### 6.2.4.1 Giới thiệu về dự án

Kubernetes (hay K8s) là một nền tảng mã nguồn mở ra mắt vào năm 2014 bởi Google, dùng để orchestrate (tự động triển khai, mở rộng và quản lý) container.

Kubernetes xuất phát từ kinh nghiệm của Google trong việc vận hành Borg và Omega, những hệ thống quản lý workload quy mô lớn. Sau đó, Google cùng Quỹ Linux (Linux Foundation) thành lập CNCF (Cloud Native Computing Foundation) để quản lý và phát triển dự án.

Kubernetes nhanh chóng trở thành chuẩn công nghiệp cho container orchestration, thay thế Docker Swarm và nhiều giải pháp khác.

---

#### 6.2.4.2. Phân tích các yếu tố

##### 6.2.4.2.1. Phạm vi (Scope)

- **Ban đầu**
  - Quản lý, triển khai và mở rộng container.
  - Tự động restart, reschedule container khi lỗi.
- **Phát triển**
  - Hỗ trợ load balancing, service discovery.
  - Quản lý tài nguyên (CPU, RAM).
  - Hỗ trợ storage, config, secret.
- **Mở rộng**
  - Trở thành nền tảng cloud-native chuẩn.
  - Hệ sinh thái plugin, operator, Helm chart.

##### 6.2.4.2.2. Tiến độ (Schedule)

- **2003 - 2013**: Google phát triển Borg, Omega (tiền thân ý tưởng).
- **2014**: Kubernetes ra mắt công khai, viết bằng Go.
- **2015**: Dự án được chuyển giao cho CNCF.
- **2016 - 2017**: Kubernetes vượt Docker Swarm và Mesos, trở thành chuẩn orchestration.
- **2018 trở đi**: Các cloud lớn (AWS, GCP, Azure) đều cung cấp dịch vụ K8s managed.
- **Hiện tại**: Kubernetes là nền tảng trung tâm của cloud-native ecosystem.

##### 6.2.4.2.3. Chi phí (Cost)

- **Ban đầu**: Google tài trợ phát triển.
- **Vận hành**: CNCF duy trì hạ tầng, hội nghị, tài liệu.
- **Doanh thu gián tiếp**: Cloud providers (AWS, Azure, GCP) thương mại hóa Kubernetes qua dịch vụ managed cluster.

**Kết luận**: Kubernetes không mang lại doanh thu trực tiếp cho CNCF, nhưng tạo giá trị khổng lồ cho hệ sinh thái cloud-native.

##### 6.2.4.2.4. Chất lượng (Quality)

- **Người dùng**: Được đánh giá linh hoạt, mạnh mẽ, nhưng đường cong học tập cao.
- **Công nghệ**: Khả năng tự healing, scaling, và orchestration toàn diện.
- **Hệ sinh thái**: Helm, Prometheus, Istio, ArgoCD, v.v.
- **Thách thức**: Độ phức tạp cao, khó triển khai và quản lý.

##### 6.2.4.2.5. Nguồn lực (Resources)

- **Nhân sự**: Được phát triển bởi Google, sau đó cộng đồng CNCF.
- **Công nghệ**: Viết bằng Go, kế thừa kinh nghiệm Borg.
- **Tài chính**: CNCF, Google, cộng đồng cloud providers tài trợ.
- **Cộng đồng**: Hàng chục nghìn contributors toàn cầu.

##### 6.2.4.2.6. Rủi ro (Risks)

- **Phức tạp**: Người dùng mới khó tiếp cận.
- **Cạnh tranh**: OpenShift (Red Hat), Nomad (HashiCorp).
- **Phụ thuộc cloud providers**: Managed services có thể "lock-in".
- **Bảo mật**: Quản lý secret, RBAC phức tạp.

#### 6.2.4.3. Bài học rút ra

- Kinh nghiệm thực tế từ Google là nền tảng thành công.
- Open-source + CNCF giúp cộng đồng phát triển mạnh.
- Chuẩn hóa orchestration tạo hệ sinh thái lớn.
- Phức tạp là rào cản: Kubernetes thành công nhưng vẫn khó dùng.
- Chiến lược phi lợi nhuận nhưng hệ sinh thái có lợi nhuận lớn (cloud vendors hưởng lợi).

Tóm lại: Kubernetes đã vượt qua Docker Swarm và Mesos để trở thành chuẩn công nghiệp cho container orchestration. Với sự hỗ trợ từ CNCF và cộng đồng toàn cầu, Kubernetes không chỉ là một dự án phần mềm mà còn là nền tảng trung tâm của cloud-native ecosystem.
