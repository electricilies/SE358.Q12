# Project Closure

# Project Closure Report

**Project Name:** Electricilies – Website for Selling Electronic Products

# Document Control

## Document Information

|                     |                                        |
| ------------------- | -------------------------------------- |
| **Document Id**     | ELEC-CLOSE-001                         |
| **Document Owner**  | Trần Nguyễn Thái Bình                  |
| **Issue Date**      | 2025-11-28                             |
| **Last Saved Date** | 2025-11-28                             |
| **File Name**       | Project Closure Report - Electricilies |

## Document Approvals

| **Role**              | **Name**              | **Date**   |
| --------------------- | --------------------- | ---------- |
| **Lecturer**          | Lê Văn Tuấn           | 2025-11-28 |
| **Project Manager**   | Trần Nguyễn Thái Bình | 2025-11-28 |
| **Quality Assurance** | Trần Nguyễn Duy Minh  | 2025-11-28 |

# 1\. Project Completion

This section identifies the criteria required to complete the project and any outstanding items which still need to be undertaken.

## 1.1. Completion Criteria

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

## 1.2. Outstanding Items

List of items that remain incomplete or require further attention after project closure.

| **Item**          | **Action**                                                                    | **Owner**              |
| ----------------- | ----------------------------------------------------------------------------- | ---------------------- |
| **Backend API**   | Finalize advanced Search, Sort, and Filter logic for large datasets.          | Nguyễn Thái Gia Nguyễn |
| **Image Upload**  | Fix Presigned URL generation logic for product image uploads in CMS.          | Trần Nguyễn Duy Minh   |
| **Documentation** | Update API documentation to reflect the latest changes in the Review Module.  | Trần Nguyễn Thái Bình  |
| **Security**      | Conduct final penetration testing on the payment gateway integration sandbox. | Trần Nguyễn Thái Bình  |

# 2\. Project Closure

This section outlines the handover of deliverables, documentation, resources, and communication.

## 2.1. Deliverables Handover

| **Deliverable**    | **Current Owner** | **Current Location**     | **New Owner**    | **Handover Activities**                                | **Date**   |
| ------------------ | ----------------- | ------------------------ | ---------------- | ------------------------------------------------------ | ---------- |
| **Source Code**    | Dev Team          | GitHub (Private Repo)    | Maintenance Team | Transfer repository ownership; Grant admin access.     | 2025-11-30 |
| **Infrastructure** | DevOps (Bình)     | Self-hosted K8s Cluster  | Ops Team         | Transfer SSH keys; Hand over `kubeconfig` and secrets. | 2025-11-30 |
| **Database**       | Backend Team      | PostgreSQL (Self-hosted) | Ops Team         | Provide connection strings; Verify backup integrity.   | 2025-11-30 |

## 2.2. Documentation Handover

| **Documentation**     | **Current Owner** | **Current Location**      | **New Owner**       | **Handover Activities**                             | **Date**   |
| --------------------- | ----------------- | ------------------------- | ------------------- | --------------------------------------------------- | ---------- |
| **Project Artifacts** | PM (Bình)         | Confluence / Google Drive | Client / Lecturer   | Archive Phase A-D reports; Export to PDF.           | 2025-11-29 |
| **Technical Docs**    | Dev Team          | GitHub Wiki / VitePress   | Maintenance Team    | Publish final API Swagger; Update deployment guide. | 2025-11-29 |
| **Design Assets**     | Designers         | Figma                     | Marketing / UI Team | Share "View/Edit" access to final design files.     | 2025-11-29 |

## 2.3. Suppliers

| **Supplier Name**   | **Contract Reference** | **Termination Activity**                            | **Release Date** | **Activity Owner**     |
| ------------------- | ---------------------- | --------------------------------------------------- | ---------------- | ---------------------- |
| **VNPay**           | Sandbox Integration    | Switch to Production Mode or Close Sandbox Account. | 2025-12-01       | Nguyễn Thái Gia Nguyễn |
| **Domain Provider** | .id.vn Registration    | Transfer domain management credentials to Client.   | 2025-12-01       | Trần Nguyễn Thái Bình  |

## 2.4. Resources

| **Resource Name**    | **Current Designation** | **Release Activity**                                       | **Release Date** | **Activity Owner**    |
| -------------------- | ----------------------- | ---------------------------------------------------------- | ---------------- | --------------------- |
| **Dev Team Members** | Developers / QA         | Release to other academic courses; Conduct exit interview. | 2025-11-30       | Trần Nguyễn Thái Bình |
| **Mini PC Server**   | K8s Master Node         | Wipe sensitive data; Return hardware to Lab/Owner.         | 2025-12-05       | Trần Nguyễn Thái Bình |
| **Network Switch**   | Infrastructure          | Disconnect and return to inventory.                        | 2025-12-05       | Trần Nguyễn Thái Bình |

## 2.5. Communication

| **Target Audience**    | **Intended Message**                                                  | **Method Used**                | **Dispatch Date** | **Dispatch Owner**    |
| ---------------------- | --------------------------------------------------------------------- | ------------------------------ | ----------------- | --------------------- |
| **Lecturer / Sponsor** | Project successfully completed; Final Report submitted.               | Email & In-person Presentation | 2025-11-28        | Trần Nguyễn Thái Bình |
| **Development Team**   | Project closed; Thank you for contributions; Lessons learned session. | Team Meeting (Retrospective)   | 2025-11-29        | Trần Nguyễn Thái Bình |
| **End Users**          | Website is live (Beta version); Feedback channel open.                | Website Banner / Email         | 2025-12-01        | Đào Duy Vinh          |

# 3\. Approval

**Name:** Trần Nguyễn Thái Bình

**Role:** Project Manager

**Signature:** _\[Signed\]_

**Date:** 28 / 11 / 2025

By signing this document, I grant approval to formally close this project and complete the hand-over activities as described above.
