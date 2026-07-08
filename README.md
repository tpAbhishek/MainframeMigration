## Mainframe Migration
Mainframe Migration to Microsoft Tech Stack

---

## About The Client
UK’s No. 1 premium lending company that is operating in UK & Ireland with 2mn+ customers across both personal and business use. The client has helped millions of businesses and individuals pay for their insurance or other financial commitments school fees, premium memberships, professional fees, membership subscriptions, commercial service charges upfront and spread the costs over instalments, instead of paying the whole premium up front since 1988.

---

## Overview

The client wanted to decommission existing I&A (Insurance and Accounting) core system which was used for servicing the recourse and non-recourse loans. The school fee loans were already on a modern .NET platform. As part of the modernization strategy, The client wanted to migrate the core system to more flexible, scalable, SOA compliant and performance-oriented technology platform. Since rest of the ecosystem was on .NET, decision was taken to modernize the core system to .NET platform. 

---

# Scope for Modernization:

- Retail Business - Web Product for Partners
- Commercial Business - Web Product for Partners
- Retail/Commercial Business - Web Product for Business Operations
- Commercial Business - Legacy/SOAP Integrations
- Legacy Batch processing and Business Logic - Retail/Commercial Business
- Include real-time integration capabilities/REST - Retail/Commercial Business

# Business Challenges
- Legacy Technology
- Increased infrastructure costs
- Slow customer response times
- Poor scalability
- Lack of centralized partner management
- No event subscription capability

The business required a modern integration platform that could provide secure, scalable, near real-time notifications while reducing unnecessary system interactions.

# Technical Challenges & Risk Mitigation

- Unavailability of mainframe documentation.
- No tools were allowed for modernization due to business controls.
- Inefficiencies of mainframe code were retained to minimize the risk
- Uncertainty about where the business logic would reside due to manual migration, leading to some business logic being incorporated into the front end.
- To mitigate business risk involved in migration to .NET platform, a fallback system was designed which also included reverse migration
- There were a lot of data dependencies preventing iterative approach, hence big bang was chosen
- Due to dependencies on the code base and processes, enhancements were kept out of scope.
---

# Solution
<img src="./Images/appFamily.png?&style=for-the-badge&logoColor=white" />
<img src="./Images/legacyFunctional.png?&style=for-the-badge&logoColor=white" />

---

# Solution Approach

- **Data Layer Migration:** The data layer, initially in mainframe file systems, was migrated to a relational database (SQL Server). Relationships were derived from the files and modeled into the new database. This migration involved extracting and loading data into new tables using SSIS packages.
- **Processing Layer Migration:** The processing part/file system was migrated to .NET. Batch jobs, which were part of the mainframe code, were migrated to SSIS packages, stored procedures, .NET, and mixed combinations. The entire migration was done manually without using any tools, as L wanted more control over the migration process.
- **Reverse Migration Scripts:** Reverse migration scripts were designed for converting RDBMS to flat files for a fallback option. This ensured that in case of total failure, they could switch back to the mainframe system.
- **Code Splitting:** The code was split into two parts: front-end system code and business logic code. Multiple parallel streams ran the as-is code conversion from the mainframe to .NET while keeping the mainframe code inefficiencies to reduce risk and testing effort. Enhancements were planned for later to minimize risk. Streams were divided based on the front end, backend, and business lines (retail, commercial).
- **Front End Translation:** Legacy screens were migrated to web-based front end using angular.js and backbone.js. These screens were interfaced with service layer.
- **Business Layer Translation:** The business layer of the mainframe was translated into a service layer. Due to manual migration, there was uncertainty about where the business logic would reside. Hence, some business logic was also incorporated into the front end, which was acceptable.

- **Testing:** Testing was done in 6-7 parallel streams. Individual environments were spun up for each stream. Both old and new systems ran in parallel for testing purposes, and reverse migration scripts were utilized for testing. With output files reverse migrated, these were compared with flat files of the mainframe system. Integration testing was also done. Testing included manual key-in to both systems, which was automated wherever possible using automation anywhere.
- **Go-live:** Once satisfied with the results, the business moved to the new system in a big bang approach. The entire data was migrated to the new system in less than 2 days. In parallel, the fallback system kept running for a month and was turned off post that. Data was translated to the fallback system overnight. In 2 months, the entire mainframe system was sunset.
- **Timelines & Teams:** The project started in 2014 and went live in 2016 (2.5 years). The project was executed in right-shore staffing where key technical resources and business analysts were onshore, and rest of the code conversion took place offshore. Project initially started with 50 resources and eventually ramped up to 200 resources. From the client side, project managers and technical architects were involved in the review.

---

# Architecture Principles

- Event-Driven Architecture
- API-First Design
- Loose Coupling
- Publish-Subscribe Pattern
- Cloud-Native Design
- Scalable Microservices
- High Availability
- Resilient Messaging

---

# Technology Stack

| Layer | Technology |
|--------|------------|
| Cloud Platform | Microsoft Azure |
| Messaging | Azure Service Bus Topics |
| Compute | Azure Functions |
| APIs | REST APIs |
| Architecture | Microservices |
| Monitoring | Azure Application Insights |
| Authentication | OAuth / API Security |
| Delivery | Agile Scrum |

---

# Resilience & Reliability

The platform was designed following cloud-native resilience patterns.

Implemented capabilities included:

- Automatic retries
- Configurable retry policies
- Timeout handling
- Dead-letter queue support
- Exception handling
- HTTP 401 authorization handling
- HTTP 500 server error handling
- Correlation IDs
- End-to-end telemetry
- Distributed logging

---

# Observability

Azure Application Insights was implemented to provide operational visibility across the platform.

Telemetry captured included:

- Event publishing metrics
- Event delivery duration
- API response times
- Function execution times
- Failure rates
- Retry counts
- Subscription activity
- End-to-end transaction tracing

---

# My Responsibilities

As the **Lead Solution Architect**, I was responsible for:

- Defining the overall platform architecture.
- Designing the event-driven integration strategy.
- Defining Azure Service Bus messaging patterns.
- Designing REST APIs and integration contracts.
- Establishing architecture standards and governance.
- Collaborating with Business Solution Architects, Product Owners, and Operations teams.
- Identifying key business KPIs and operational metrics.
- Guiding engineering teams throughout Agile delivery.
- Reviewing solution designs and development artefacts.
- Leading architecture reviews and technical governance.
- Defining resilience, scalability, and observability requirements.

---

# Business Outcomes

✅ Decommissioned Automation Anywhere and Oracle (cost)

✅ Increase in transaction capacity by 30%

✅ Improvement in collections efficiency by 30%

✅ Increased business up time from 98% to 99.9%

✅ Trustpilot rating from 2.5 to 4.5

✅ Reduced onboarding duration from 2 weeks to 2 days

✅ Loan authorization duration from 72 to 24 hours 

✅ Reduction in contact center FTE by 50% 

✅ Enabled modern integration services using REST APIs.

✅ Enabled near real-time loan application notifications.

✅ Paved the way for retail and commercial portal consolidation.

✅ Recognized as a milestone modernization initiative by business leadership.

---

# Key Learnings

This project demonstrated how event-driven integration platforms can significantly improve scalability, customer experience, and operational efficiency.

Key architectural learnings included:

- Leverage Cloud technologies to modernize legacy systems is cost effective.
- Cloud-native resilience patterns improve platform reliability.
- Observability is essential for distributed systems.
- Self-service onboarding reduces operational overhead while improving partner experience.

---

# Skills Demonstrated

- Solution Architecture
- Enterprise Integration
- Event-Driven Architecture
- Publish-Subscribe Pattern
- Microsoft Azure
- Azure Service Bus
- Azure Functions
- Microservices
- REST APIs
- Partner Integration
- API Management
- Cloud Architecture
- Distributed Systems
- Platform Engineering
- Resilience Engineering
- Azure Application Insights
- Technical Leadership
- Architecture Governance
- Stakeholder Management
- Agile Delivery

