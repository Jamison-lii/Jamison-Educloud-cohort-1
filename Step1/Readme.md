
#  **10 Layers of the RentIt Project**


## **Layer 1 — Client Apps (Frontend)**

What the user interacts with

**Components**

* Mobile App (React Native)
* Web App (React)
* UI Navigation
* Authentication screens
* Rental and listing screens

**Cloud Role**

* Static hosting (Web)
* Mobile builds
* CDN distribution

## **Layer 2 — API Gateway / Edge Routing**

Front door of the backend services

**Purpose**

* Route API calls
* Authentication enforcement
* Throttling & security


## **Layer 3 — Authentication & Identity**

User identity and access control

**Purpose**

* Register users
* Login
* Multi-factor authentication
* Verification badges


## **Layer 4 — Core Business Logic**

Handles all GetIt processes

**Examples**

* Listings creation
* Searching and filtering
* Rental requests
* Approvals
* Returns
* Disputes
* Payments + escrow logic


## **Layer 5 — Database / Storage**

Stores all the data

**What it stores**

* Users
* Listings
* Rentals
* Reviews
* Disputes
* Payments
* Verification docs
* Logs


## **Layer 6 — File Storage**

For photos and documents

**Examples**

* Item photos
* Identity documents
* Dispute evidence
* Chat image uploads


## **Layer 7 — Payments & Escrow**

Secure financial operations

**Examples**

* Holding deposits
* Releasing payments
* Billing cycles
* Refunds


## **Layer 8 — Messaging & Notifications**

Real-time or asynchronous alerts

**Examples**

* Rental request notifications
* Return reminders
* Dispute status updates
* In-app messages


## **Layer 9 — Monitoring & Logging**

Keeping the system healthy

**What it does**

* Performance tracing
* Error logging
* Usage analytics
* Audit logs


## **Layer 10 — DevOps / CI CD / Security**

Automated builds and secure delivery

**Examples**

* Automated deployments (CI/CD)
* HTTPS enforcement
* Secret management
* Role access policies


# **Cloud Services to Build Each Layer**

##  **AWS Cloud Services**

| Layer                        | AWS Service                                                   |
| ---------------------------- | ------------------------------------------------------------- |
| Layer 1 – Client Apps        | **CloudFront + S3 (Web), React Native stores on App stores**  |
| Layer 2 – API Gateway        | Amazon API Gateway                                            |
| Layer 3 – Authentication     | **Amazon Cognito**                                            |
| Layer 4 – Business Logic     | **AWS Lambda**, **AWS Fargate / ECS**                         |
| Layer 5 – Database           | **Amazon DynamoDB** / **RDS (PostgreSQL)**                    |
| Layer 6 – File Storage       | **Amazon S3**                                                 |
| Layer 7 – Payments           | Integrate momo or fapshi with API Gateway           |
| Layer 8 – Messaging          | **AWS SNS**, **AWS Pinpoint**, **WebSockets** via API Gateway |
| Layer 9 – Monitoring         | **CloudWatch**, **X-Ray**, **CloudTrail**                     |
| Layer 10 – DevOps / Security | **CodePipeline**, **IAM**, **Secrets Manager**                |




