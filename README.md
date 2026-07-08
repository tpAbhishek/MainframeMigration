# 🌐 Mainframe Migration
Mainframe Migration to Microsoft Tech Stack

---

## About The Client
UK’s No. 1 premium lending company that operating in UK & Ireland with 2mn+ customers across both personal and business use. The client has helped millions of businesses and individuals pay for their insurance or other financial commitments school fees, premium memberships upfront and spread the costs over instalments, instead of paying the whole premium up front since 1988. The client also provides the finance to pay annual costs such as professional fees, membership subscriptions, commercial service charges and school fees

---

## Overview

The client wanted to decommission existing I&A (Insurance and Accounting) core system which was used for servicing the recourse and non-recourse loans. The school fee loans were already on a modern .NET platform. As part of the modernization strategy, The client wanted to migrate the core system to more flexible, scalable, SOA compliant and performance-oriented technology platform. Since rest of the ecosystem was on .NET, decision was taken to modernize the core system to .NET platform. 

---

# Scope for Modernization:

I&A Recourse - Retail Business
I&A Non-recourse - Commercial Business
I&A Interactive - Retail/Commercial Business
PDF/XML - Commercial Business 
Legacy Batch processing and Business Logic - Retail/Commercial Business
Include real-time integration capabilities - Retail/Commercial Business

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

# Solution Architecture

A cloud-native, event-driven platform was designed using Microsoft Azure services.

## High-Level Workflow

<img src="./Images/EnterpriseEventGateway.png?&style=for-the-badge&logoColor=white" />

---

# Platform Modules

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

