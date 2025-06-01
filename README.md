# airbnb-clone-project


## 📖 Project Overview

The **Airbnb Clone Project** is a full-stack web application that replicates the core functionalities of the Airbnb platform. Built using **Python, JavaScript, Django, MySQL**, and **GraphQL**, this project is designed to provide a hands-on learning experience in developing scalable, secure, and production-ready applications. It emphasizes backend architecture, database design, API development, and team collaboration.

### 🎯 Project Goals

* Secure user registration and authentication
* Property listing creation and management
* Booking system with reservation tracking
* Integrated payment processing
* User reviews and property ratings
* Optimized data storage and retrieval

## 🛠️ Tech Stack

* **Django & Django REST Framework** – Backend and APIs
* **PostgreSQL** – Data storage
* **GraphQL** – Flexible data querying
* **Celery & Redis** – Asynchronous tasks and caching
* **Docker** – Environment consistency
* **CI/CD Pipelines** – Automated testing and deployment

## 👥 Team Roles
🔧 Backend Developer
Responsible for building and maintaining the server-side of the application. Implements API endpoints, designs database schemas, and ensures the core business logic functions smoothly and securely.

🗃️ Database Administrator (DBA)
Oversees the structure and performance of the database. Handles schema design, indexing strategies, data migrations, and ensures efficient data storage and retrieval.

🚀 DevOps Engineer
Manages the deployment pipeline and infrastructure. Sets up Docker environments, CI/CD workflows, monitors system performance, and ensures the application is scalable and reliably deployed.

✅ QA Engineer
Ensures all backend features meet the required standards through rigorous testing. Designs and runs automated/manual tests, identifies bugs, and collaborates with the team to maintain code quality and functionality.

## 🗄️ Database Design

**User**
Key fields: id, username, email, password_hash, role.
Relationships: A user can have multiple properties and bookings.

**Property**
Key fields: id, user_id, title, address, price_per_night.
Relationships: A property belongs to one user and can have multiple bookings and reviews.

**Booking**
Key fields: id, user_id, property_id, start_date, end_date.
Relationships: A booking is linked to one user and one property.

**Review**
Key fields: id, user_id, property_id, rating, comment.
Relationships: A review is written by one user for one property.

**Payment**
Key fields: id, user_id, booking_id, amount, payment_status.
Relationships: A payment is made by one user for one booking.

## 🧩 Feature Breakdown
**User Management:** Enables secure registration, authentication, and profile management, with different roles for hosts and guests, ensuring access control and personalization.

**Property Management:** Allows hosts to create, update, and delete property listings, ensuring users have up-to-date options for booking.

**Booking System:** Lets guests reserve properties for specific dates, managing reservations and booking details seamlessly.

**Payment Processing:** Facilitates secure payments for bookings, recording transaction amounts and payment statuses for smooth financial exchanges.

**Review System:** Allows users to leave ratings and reviews for properties, building trust and helping future users make informed decisions.

**Data Optimization:** Ensures efficient data storage and fast retrieval, keeping the app responsive and scalable.

## 🔒 API Security
Authentication: Uses token-based authentication (JWT) to verify user identity, ensuring only authorized users access protected resources.

Authorization: Implements role-based access control (RBAC) to restrict actions based on user roles (e.g., guests vs. hosts), preventing unauthorized access to sensitive data.

Rate Limiting: Limits the number of requests a user can make within a set time, protecting the system from overloading and ensuring availability.

Data Encryption: Encrypts sensitive data both in transit (via HTTPS) and at rest, ensuring the confidentiality and integrity of user information.

Payment Security: Utilizes secure, third-party payment gateways to handle transactions, ensuring compliance with industry security standards and protecting payment details.

## 🚀 CI/CD Pipeline
CI/CD (Continuous Integration/Continuous Deployment) automates the integration of code changes and their deployment to production, ensuring reliable and frequent updates. It helps identify bugs early, reduces manual tasks, and speeds up delivery.
Tools:

GitHub Actions: Automates testing and deployment within GitHub repositories.

Docker: Ensures consistent environments through containerization.

Jenkins: Automates integration and delivery pipelines.

CircleCI: Automates the build, test, and deploy processes.
