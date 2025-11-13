# Michael Hanley

[me@hanleym.com](mailto:me@hanleym.com)

Principal Software Engineer with 15+ years of experience designing distributed systems, CI/CD infrastructure, and backend services in Rust, Go, and C#.
Deep expertise in NixOS, Kubernetes, and cloud, on-prem, and hybrid architectures.
Architect and hands-on engineer with a proven record of improving reliability, cutting costs, and leading high-impact technical transformations.


## Skills

- **Languages:** Rust, Go, C#, TypeScript/JavaScript, Python
- **Data Systems:** PostgreSQL, MySQL/TiDB, SurrealDB, TiKV, DynamoDB, Prometheus, Redis
- **Protocols & Messaging:** HTTP, GraphQL, gRPC/Protobuf, OpenTelemetry, MQTT, JSON, Syslog, SQS, SNS
- **Infrastructure & DevOps:** Nix/NixOS, Kubernetes, Docker, Terraform, AWS, Linux



## Experience

### Calamu - Remote
#### Principal Software Engineer - November 2023 to October 2025

- Built a fully declarative Nix-based CI/CD system for both cloud and on-prem deployments.
  - Leveraged Nix, NixOS GitHub self-hosted runners, distributed binary caches, and remote (distributed) builds to generate and deploy NixOS configurations, Docker images, Terraform, and Kubernetes YAML.
  - Achieved reproducible, deterministic builds with significant speed and reliability gains.
- Discovered and demonstrated a critical vulnerability, responsibly disclosed it, and led a complete architectural redesign.
  - Delivered high-performance cross-platform implementations in Rust and C#.
  - Eliminated the flaw and improved throughput.
- Developed a TUI for provisioning on-prem clusters.
  - Implemented in Rust with Nix-based deployment.
  - Reduced provisioning time to under 15 minutes.
- Developed a distributed execution engine in C#, then built migration and purge features on top of it.
  - Implemented durable queuing, retries, and coordination between backend services and distributed agents.
  - Supported seamless data migration across AWS S3, GCP, Azure Blob, and S3-compatible services.
- Built a Rust-based benchmarking suite for comparing S3-compatible services.
  - Measured performance data for regression tracking and product validation.
- Re-architected infrastructure to replace an expensive and fragmented AWS stack (Fargate, Lambda, DynamoDB, Neptune).
  - Migrated to Kubernetes and SurrealDB/TiKV, achieving a 10x cost reduction and multi-cloud/on-prem portability.
  - Featured in SurrealDB's case study: [Storing cybersecurity data at scale with SurrealDB](https://surrealdb.com/customer/calamu)

### Tably - Remote
#### Senior Software Engineer - August 2022 to May 2023

- Developed a Notion-style block editor for an interactive web-based computing platform (conceptually similar to Jupyter Notebook).
  - Implemented in Rust using Sycamore and a proprietary operational transform engine.
  - Delivered real-time synchronization and structured data editing across users.

### KnowBe4 - Hybrid (Clearwater, FL)
#### Senior Software Engineer - November 2017 to July 2022

  
- Developed a replacement SCIM identity provisioning service to support massive traffic bursts.
  - The previous open-source system frequently ran out of memory under load and required replacement.
  - Proposed and led the adoption of Rust for the project due to its performance and predictable memory management.
  - Designed and implemented a Rust-based Lambda + DynamoDB replacement handling 2.5 M requests/day and >7 K/min bursts, isolated tenant issues, and reduced AWS costs tenfold.
  - Featured in: [Software Architecture and the Art of Doing it Right the First Time](https://www.knowbe4.com/careers/blogs/engineering/software-architecture-and-the-art-of-doing-it-right-the-first-time)
- Delivered the backend for [CARA](https://www.knowbe4.com/compliance-audit-readiness-assessment), a [CMMC](https://www.acq.osd.mil/cmmc/) compliance readiness tool.
  - Took over from a struggling team and met a hard deadline.
  - Implemented with Python, GraphQL, API Gateway, Lambda, and S3.
  - Adopted as the foundation for the team's future microservices.
- Built internal integration microservices to continuously scan customer domains via [EEC](https://www.knowbe4.com/email-exposure-check/) and synchronize results to product and data pipelines.
  - Implemented in Go using Step Functions, Lambda, SNS, and S3.
  - Runs ~67 K state machines to scan 130 K+ domains each month.
- Rebuilt [PhishER](https://www.knowbe4.com/products/phisher)'s VirusTotal integration to support complex upstream rate limits and reliability constraints.
  - Implemented in Go using Lambda and DynamoDB.
  - Processes > 3 M requests and 8 M invocations/month.
- Contributed to the design and migration of the internal email delivery system.
  - Led migration from MySQL to PostgreSQL to address transactional and performance limitations.
  - Implemented in Go using Fargate, Aurora, and SQS.
  - Used across the company to send > 40 M emails/month.
- Created the [PhishER: Threat Map](https://map.knowbe4.com/): a live map visualizing global phishing activity.
  - Developed full stack in Go + JavaScript (VueJS & Canvas) with Fargate, SQS, and WebSockets.
  - Handled > 3 M subscriptions before being replaced on the homepage with a simulated view.
- Engineered core backend services for [PhishER](https://www.knowbe4.com/products/phisher), including a rule evaluation engine, YARA integration, and Syslog integration.
  - Implemented using Go, gRPC/Protobuf, libyara, Fargate, ELB/NLB, and consistent hashing for distributed load balancing.
  - Co-inventor on U.S. Patents: [US10812507B2](https://patents.google.com/patent/US10812507B2/), [US11108791B2](https://patents.google.com/patent/US11108791B2/), [US11902302B2](https://patents.google.com/patent/US11902302B2/) - Systems and methods for efficient combining of characteristic detection rules.
- Developed backend services for several public tools: [Email Exposure Check](https://www.knowbe4.com/email-exposure-check/), [Weak Password Test](https://www.knowbe4.com/weak-password-test), [Breached Password Test](https://www.knowbe4.com/breached-password-test), [Password Exposure Test](https://www.knowbe4.com/password-exposure-test), [Second Chance](https://www.knowbe4.com/second-chance), and [Multi-factor Authentication Security Assessment](multi-factor-authentication-security-assessment).
  - Implemented in Go using Fargate, ELB/NLB, gRPC/Protobuf, and cryptographic libraries.

### nThrive - Remote
#### Senior Systems & Software Engineer - June 2012 to November 2017

- Created a proprietary interactive lesson format used in 1.6 K+ lessons taken by millions of healthcare professionals.
  - Implemented in JavaScript using React, Redux, Material Design, SCORM, and xAPI.
- Automated content packaging using a build system written in Go integrating ffmpeg, ImageMagick, Ghostscript, and inotify.
  - Produced 1 K+ lessons with 3.6 K+ interactive elements, dramatically improving productivity.
- Built a mobile application (iOS and Android) to allow searching complex hierarchies of medical codes in JavaScript (Titanium).
  - Ranked #67 globally and #1 in Medical on the App Store for several months.
- Modified and administered an existing learning management system (LMS), allowing it to scale to hundreds of thousands of learners.
  - Transitioned from PHP to Go microservices, introducing Redis caching, HAProxy/Nginx load balancing, and Ceph distributed storage.
- Developed a web app for live and on-demand streaming of medical seminars.
  - Frontend in JavaScript using AngularJS, VideoJS, and xAPI.
  - Backend in Go using Authorize.net, RethinkDB, and ffmpeg.

### Focus School Software - St. Petersburg, Florida
#### Software Engineer - March 2010 to June 2012
- Optimized core data manipulation functions, replacing inefficient and insecure eval() logic with recursion for an application-wide ~16% performance gain.
- Fixed critical SQL injection vulnerabilities by replacing regex-based escaping with parameterized database calls.
- Automated generation of Department of Education reports in PHP, simplifying compliance workflows.
- Integrated memcached caching to cut query load and reduce page times by up to 35%.

