# Michael Hanley

[me@hanleym.com](mailto:me@hanleym.com)

As a dedicated and driven Software Engineer with 15 years of experience, my journey has been defined by a relentless pursuit of confronting intricate technical challenges through system and software development. My career has been marked by a commitment to continuous learning, staying at the forefront of emerging technologies, and weaving them into the fabric of my extensive expertise. With a proven ability to manage projects effectively, conduct thorough testing, provide comprehensive support, and create user-friendly technical documentation, I bring a holistic approach to software engineering. This combination of passion, expertise, and adaptability allows me to deliver robust and creative solutions, making me a valuable asset to any team.

## Skills
- **Languages:** Rust, Go, TypeScript, JavaScript, Python, Dart, C#, Lua
- **Databases:** SQL (PostgreSQL & MySQL), DynamoDB, ElasticSearch, InfluxDB, SurrealDB, RethinkDB, MongoDB
- **Protocols / Serialization:** HTTP, GraphQL, gRPC / Protobuf, MQTT, Syslog, JSON
- **Messaging:** NATS, SQS, SNS
- **Operating Systems:** NixOS, Arch, Ubuntu / Debian, RHEL / Fedora, MacOS, Windows
- **Infrastructure:** Nix, Kubernetes, Containers, AWS, Terraform

## Experience

### Calamu - Remote
#### Senior Software Engineer - November 2023 to Present

 - Designed and developed a a Nix CI/CD build system to replace existing shell scripts that were used to copy directly from developer machines to production environments. These changes ensure builds / deployments are immutable and deterministic.
 - Helped replace multiple AWS services (Fargate, Lambda, DynamoDB, Neptune, etc...) with Kubernetes and SurrealDB. These changes massively reduced operating costs and enabled the product to be deployed to multi-cloud and on-premises environments. 
 - Individually designed and developed a Rust S3 benchmark tool to allow us to more accurately see our product's performance improvements and compare against AWS and other S3 compatible providers.

### Tably - Remote
#### Senior Software Engineer - August 2022 to May 2023

- Developed a [Notion](https://www.notion.so/) style (block-based) editor for use in a web-based interactive computing platform (vaguely similar to [Jupyter Notebook](https://jupyter.org/)).
  - Written in Rust, utilizing [Sycamore](https://sycamore-rs.netlify.app/) and a proprietary (planned to be open-source) operational transform implementation.

### KnowBe4 - Hybrid (Clearwater, Florida, US)
#### Senior Software Engineer - November 2017 to July 2022
  
- Designed and developed a replacement [SCIM](http://www.simplecloud.info/) implementation capable of handling large bursts of traffic.
  - The previous system (a modified open-source solution) was unable to handle the throughput required by our larger customers. The service would run out of memory due to a combination of architecture and memory management oversights, causing outages and incurring considerable costs.
  - Proposed and led the adoption of Rust for the replacement due to its solid performance and predictable memory management.
  - Written in Rust, utilizing API Gateway, Lambda, and DynamoDB.
  - Upon release of the project, it handled 2.5 million invocations per day with bursts of over 7 thousand invocations in a one-minute window. Additionally, the serverless architecture isolated issues caused by individual customers and reduced costs by an order of magnitude.
- Designed and developed the backend for [Compliance Audit Readiness Assessment (CARA)](https://www.knowbe4.com/compliance-audit-readiness-assessment), a free tool allowing prospective clients to assess their readiness to meet [CMMC](https://www.acq.osd.mil/cmmc/) requirements.
  - Given my track record of rapidly and reliably delivering numerous similar projects, was asked to step in and build the backend for a team that was struggling and unlikely to make an important and inflexible deadline.
  - Written in Python, utilizing GraphQL, API Gateway, Lambda, and S3.
  - The project was completed by the deadline, and the implementation was clean & robust enough to be handed off successfully and eventually be adopted as the starting point for the team's future microservices.
- Designed and developed internal integration microservices to continually scan existing customers' domains with [EEC](https://www.knowbe4.com/email-exposure-check/) and synchronize the results to both the product and data science pipelines.
  - Written in Go, utilizing Step Functions, Lambda, SNS, and S3.
  - Runs about 67 thousand state machines to scan over 130 thousand domains each month.
- Designed and developed a replacement [VirusTotal](https://www.virustotal.com/) integration for [PhishER](https://www.knowbe4.com/products/phisher) allowing customers to reliably scan URLs and attachments sent to PhishER with VirusTotal.
  - The previous system wasn't robust enough to handle the various constraints (imposed by both the business requirements and VirusTotal rate limiting).
  - Written in Go, utilizing Lambda, and DynamoDB.
  - Handles over 3 million requests with over 8 million Lambda invocations per month.
- Assisted with the internal email service design and migration.
  - Contributed to design decisions and performed code reviews.
  - Ported the project from MySQL to PostgreSQL due to limitations found in MySQL around performance and transactions.
  - Written in Go, utilizing Fargate, Arora, and SQS.
  - Used across the company to send over 40 million emails per month.
- Individually designed and developed (frontend and backend) the [PhishER](https://www.knowbe4.com/products/phisher): [Threat Map](https://map.knowbe4.com/); a live map of phishing attacks targeted at our customers.
  - Written in Go & JavaScript, utilizing Fargate, SQS, WebSockets, VueJS, and Canvas.
  - Used primarily for marketing. Handled over 3 million subscriptions the final month it was on the company homepage (replaced by a simulated view with a link to the live view to reduce costs).
- Designed and developed many of the core backend services for [PhishER](https://www.knowbe4.com/products/phisher); specifically the rule evaluation engine, [Yara](https://virustotal.github.io/yara/) integration, and Syslog integration.
  - Written in Go, utilizing [Consistent Hashing](https://en.wikipedia.org/wiki/Consistent_hashing), [Fargate](https://aws.amazon.com/fargate/), [ELB/NLB](https://aws.amazon.com/elasticloadbalancing/network-load-balancer/), [gRPC](https://grpc.io/), [Protobuf](https://developers.google.com/protocol-buffers), [libyara](https://yara.readthedocs.io/en/stable/capi.html), and the TCP, UDP, and TLS packages from the standard library.
  - Helped invent and patent ([US10812507B2](https://patents.google.com/patent/US10812507B2/)) a method for efficiently processing characteristic detection rules in a rule set.
- Designed and developed the backend services for many of the free tools created at KnowBe4, including [Email Exposure Check](https://www.knowbe4.com/email-exposure-check/) v2, [Weak Password Test](https://www.knowbe4.com/weak-password-test) v2, [Breached Password Test](https://www.knowbe4.com/breached-password-test), [Password Exposure Test](https://www.knowbe4.com/password-exposure-test), [Second Chance](https://www.knowbe4.com/second-chance) v2, and [Multi-factor Authentication Security Assessment](multi-factor-authentication-security-assessment)
  - Written in Go, utilizing [Fargate](https://aws.amazon.com/fargate/), [ELB/NLB](https://aws.amazon.com/elasticloadbalancing/network-load-balancer/), [gRPC](https://grpc.io/), [Protobuf](https://developers.google.com/protocol-buffers), and may of the cryptography packages from the standard library.

### FinThrive - Remote
#### Senior Systems & Software Engineer - June 2012 to November 2017
- Designed and developed a proprietary lesson format allowing for engaging and interactive education to reach millions of learners on a wide variety of devices.
  - Written in JavaScript, utilizing React, Redux, Material Design, SCORM, and xAPI.
  - Used for over 1,696 lessons taken by millions of medical professionals.
- Designed and developed an automated lesson building and packaging system that increased productivity dramatically.
  - Written in Go, utilizing ffmpeg, imagemagick, ghostscript, and inotify.
  - Used to build 1,073 lessons with a combined 3,619 interactives.
- Designed and developed a mobile (iOS and Android) application to simplify and search complex hierarchies of medical codes.
  - Written in JavaScript, utilizing Titanium.
  - Reached 67th Globally and 1st in Medical on the App Store for several months.
- Modified and administered an existing learning management system (LMS) allowing it to scale to hundreds of thousands of learners.
  - Initial modifications in PHP; later, a Go microservice architecture was adopted.
  - Scaling required rewriting core logic, as well as implementing load balancing (HAProxy + Nginx), caching (Redis), and a distributed filesystem (Ceph.)
- Contributed to a mobile ready web application allowing physicians and hospital staff to purchase and stream educational seminars and other videos live or on-demand.
  - Backend in Go, utilizing Authorize.net, RethinkDB (migrated from MongoDB,) and ffmpeg.
  - Frontend in JavaScript, utilizing AngularJS, VideoJS, and xAPI.

### Focus School Software - St. Petersburg, Florida
#### Software Engineer - March 2010 to June 2012
- Modified core database functions significantly increasing the performance of the entire application.
  - Used recursion to replace existing calls to `eval()`.
  - Performance increase of ~16% across the application.
- Modified escaping and input libraries to patch security vulnerabilities.
  - Identified and demonstrated vulnerabilities in the existing regex escaping strategy and led the effort to use the appropriate database escape calls.
- Developed algorithms used to automatically generate, compare, and update reports sent to the department of education majorly enhancing usability and increasing efficiency.
  - Written in PHP; interfaced with legacy government mainframe systems.
- Implemented memcached to reduce the total number of queries executed.
  - Reduced page load times by as much as 35%.

