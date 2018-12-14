# DataOps

Notes, labs and general content around DataOps (aka "DevOps for Data Science & Engineering", aka "Agile Data Science").  This repository will serve as a source for developing DataOps practices in an Organization, leveraging best practices for simplified, automated and idempotent (re)deployments.

## Areas to consider
### Data Estate
1. Ingestion
1. Raw Data Storage
1. Raw Data Processing
1. Refined Data Stroage
1. Refined Data Access
1. Data Feedback Loop

### Security
1. AAA (Authentication, Authorization, Accounting)
  - Login/Credentialing (Authentication)
  - RBAC/ACLs (Authorization)
  - Monitoring/Logging/Auditing (Accounting)
1. Data Security at Rest (Data Storage Encryption)
  - Encrpytion Key (Password) Rotation
    - Time Bound Key Rotation
    - One Time Passwords
  - Encryption Key Storage
1. Data Security in Transit (Data Encryption in Transit w/SSL, mTLS etc)
  - Service Discovery and Service Access Control Policies (Intents)

### DevOps
1. Infrastructure as Code
  - Repeatable Idempotent Deployment of App/Infra and Data (AI/ML/AA/DB/Storage) Services
1. Data Model (Code) Versioning
1. Data Source Versioning
1. Automated Build
1. Data Model Testing
1. Automated/Gated Releases
1. Telemetry