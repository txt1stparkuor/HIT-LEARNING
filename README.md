# 🎓 HIT SYMPHONY - Club Management Platform

![Java](https://img.shields.io/badge/Java-17-blue) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-brightgreen) ![ReactJS](https://img.shields.io/badge/ReactJS-19.x-blue?logo=react) ![MySQL](https://img.shields.io/badge/MySQL-8+-orange?logo=mysql) ![Docker](https://img.shields.io/badge/Docker-Ready-blue?logo=docker)

> An all-in-one educational and management platform built for the **HIT (Haui Information Technology)** university club. 

This repository serves as an overview of the HIT Symphony full-stack project. To dive into the codebases, please visit the specific repositories below.

### 📌 Quick Links
* 🎨 **UI/UX Design:** [Figma Workspace](https://www.figma.com/design/vI7ilYugZQZ8GUxwJtpq12/HIT---Symphony---Design?node-id=27-26&t=viIK8WCRXO19vGm2-0)
* 💻 **Frontend Source Code:** [HIT-SYMPHONY/frontend_symphony_app](https://github.com/HIT-SYMPHONY/fontend_symphony_app/tree/develop)
* ⚙️ **Backend Source Code:** [HIT-SYMPHONY/Backend-Symphony](https://github.com/HIT-SYMPHONY/Backend-Symphony/tree/develop)

---

## 📖 About The Project

Managing a large university IT club requires serious organization. **HIT Symphony** was built to provide a professional, centralized space for club members to interact. 

Instead of relying on scattered Facebook groups or Google Drives, this platform allows students to access study materials, submit homework, participate in club-hosted coding competitions, and receive real-time notifications about upcoming classes.

### ✨ Key Features

* **📚 Study Material & Class Management:** Organizers can create classes, schedule specific study sessions, and upload relevant materials for students to view.
* **📝 Homework & Grading System:** Leaders can assign homework, and students can submit their work directly through the platform for grading.
* **🏆 Competition Hub:** A dedicated module for hosting club competitions, managing participants, and handling submissions.
* **🔐 Secure Auth & Role Management:** Robust RBAC (Role-Based Access Control) using JWT (`AccessToken` & `RefreshToken`) and Spring Security to separate Admins, Leaders, and Students.
* **🔔 Real-time Notifications:** WebSocket integration to instantly notify classes or competitors about updates.

---

## 🛠️ System Architecture & Tech Stack

The platform is separated into a React frontend client and a Spring Boot backend server.

### Frontend ([View Code](https://github.com/HIT-SYMPHONY/fontend_symphony_app/tree/develop))
* **Core:** React.js (v19) & Vite
* **State Management & Data Fetching:** Redux Toolkit, React Query (`@tanstack/react-query`)
* **Styling & UI:** Tailwind CSS, Ant Design (`antd`), Sass
* **Routing & HTTP:** React Router v7, Axios
* **Forms & Validation:** React Hook Form, Formik, Yup
* **Real-time Client:** StompJS (WebSocket integration)
* **Utilities:** Tiptap (Rich Text Editor), Swiper (Carousels), React Hot Toast

### Backend ([View Code](https://github.com/HIT-SYMPHONY/Backend-Symphony/tree/develop))
* **Core:** Java 17, Spring Boot 3.x
* **Security & Auth:** Spring Security (OAuth2), JWT
* **Real-time Comm:** Spring WebSocket
* **Database & ORM:** MySQL 8+, Spring Data JPA, Hibernate
* **Utilities:** Spring Mail (Email notifications), Bucket4j (Rate limiting), Cloudinary (Image/File hosting)

### DevOps & Infrastructure
* **Deployment:** Digital Ocean VPS
* **Containerization:** Docker
* **Code Quality:** SonarQube

---
