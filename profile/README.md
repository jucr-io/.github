<!-- markdownlint-disable -->
  <a href="https://jucr.com/">
    <img src="https://github.com/jucr-io/.github/blob/adding-public-info/banner/image_banner.png?raw=true" alt="Project Banner"/>
  </a>
<br/>
<p align="left">
  <a href="https://jucr-io.slack.com">
    <img src="https://upload.wikimedia.org/wikipedia/commons/b/b9/Slack_Technologies_Logo.svg" alt="Slack Community" width="80" height="20"/>
  </a>
</p>
<!-- markdownlint-restore -->

![Last Update](https://img.shields.io/github/last-commit/jucr-io/.github/main)
[![Code Analysis](https://github.com/jucr-io/.github/actions/workflows/ci.yml/badge.svg)](https://github.com/jucr-io/.github/actions/workflows/ci.yml)

# We are JUCR ⚡️

JUCR is on a mission to accelerate the global adoption of electric vehicles by providing accessible and user-friendly charging solutions. We are dedicated to creating the most exciting and seamless experience for every electric car driver, enabling them to fully embrace the freedom and possibilities of e-mobility without any limitations.

Based in the vibrant city of **Berlin**, our company thrives in a hub of innovation and culture. Our diverse team consists of brilliant minds from over **20 different nationalities**, bringing together a rich variety of cultures, ideas, and expertise. This diversity fuels our creativity and allows us to approach challenges from unique perspectives, fostering innovation at every level of the organization.

At JUCR, we take pride in building everything in-house. This means we have full control over our products and services, ensuring the highest quality and security standards. From designing and manufacturing the PCBs that power our charging stations to developing the firmware for microcontrollers, crafting our entire backend platform, and creating intuitive mobile applications, we handle it all. 
This vertical integration allows us to optimize every aspect of our technology stack, providing a seamless and cohesive experience for our users.

## Languages We Use

We believe in using the right tool for each specific problem, which is why we embrace a variety of programming languages and technologies. Our multilingual approach allows us to leverage the strengths of each language, resulting in efficient and effective solutions.

- **Rust**: Utilized extensively in our embedded systems and backend services, Rust offers memory safety and high performance. Its zero-cost abstractions and fearless concurrency make it ideal for systems programming where reliability is paramount.
  
- **TypeScript**: Used in our backend development, TypeScript brings static typing to JavaScript, enhancing code quality, maintainability, and scalability. It helps us catch errors early and build robust APIs and services. For many years, we've been maintaining our own framework to reduce the hell of the dependencies usually associated to this ecosystem.

- **HCL**: Employed for infrastructure as code (IaC) with tools like Terraform, HCL allows us to define and provision our infrastructure in a declarative way, ensuring consistency and repeatability across environments.

- **Swift**: For our iOS frontend development Swift provides a modern, fast, and safe programming language. It enables us to build high-performance, user-friendly mobile applications with a native experience on Apple devices.

- **Kotlin**: Used in our Android frontend development, Kotlin offers concise syntax and interoperability with Java. It allows us to create powerful and expressive applications while reducing boilerplate code.

- **React**: Leveraged in our web frontend development, React enables us to build dynamic and responsive user interfaces. It's component-based architecture promotes reusability and efficient rendering, enhancing user engagement and experience.

## Our Toolchain & Architecture

Our platform is architected using a microservices approach, consisting of over **50 microservices** that communicate in a fully decoupled, event-driven manner. This architecture allows for:

- **Scalability**: Services scale independently based on demand, ensuring optimal performance.
- **Resilience**: The decoupled nature reduces the impact of failures, enhancing system reliability.
- **Flexibility**: Teams can develop, deploy, and update services independently, accelerating innovation.

The toolchain that powers our platform includes, but is not limited to:

- **Kubernetes (EKS)**: We utilize Amazon EKS to orchestrate our containerized applications, enabling us to manage and scale our microservices efficiently in a cloud-native environment. Kubernetes provides automated deployment, scaling, and management of containerized applications, ensuring high availability and resilience.

- **Kafka**: As a distributed streaming platform, Kafka enables us to handle real-time data feeds with high throughput and low latency. It's the backbone of our event-driven architecture, facilitating seamless communication between services.

- **GraphQL**: We use GraphQL to build efficient and flexible APIs. It allows clients to request exactly the data they need, reducing over-fetching and under-fetching of data, which optimizes network usage and improves performance.

- **Terraform**: With Terraform as our choice for infrastructure as code, we provision and manage our infrastructure resources across various cloud providers consistently and automatically. It enhances our ability to deploy scalable and reliable infrastructure rapidly.

- **DynamoDB**: AWS DynamoDB offers a fast and flexible NoSQL database service for applications that need consistent, single-digit millisecond latency at any scale. It's ideal for handling high-throughput workloads and ensuring low-latency responses.

- **MongoDB**: As a NoSQL database, MongoDB provides flexibility in handling unstructured data. It supports our need for scalable, high-performance data storage, especially for applications that require rapid development cycles.

- **ELK Stack**: We leverage the ELK stack (Elasticsearch, Logstash, and Kibana) for centralized logging and monitoring. We primarily use Elasticsearch for performative queries, enabling us to quickly search and analyze large volumes of data. This setup improves our ability to troubleshoot and maintain system performance.

- **Apache Flink**: Flink is used for real-time stream processing, enabling us to perform complex event processing and analytics on data streams with low latency and high throughput. This allows us to make informed decisions based on real-time insights.

- **Datadog**: For observability and monitoring, we utilize Datadog to track application performance, monitor infrastructure health, and gain insights into user behavior. Datadog provides powerful analytics and visualization tools, allowing us to ensure the reliability and efficiency of our services.

In addition to our toolchain, our architecture is heavily influenced by the following principles:

- **Domain-Driven Design (DDD)**: We structure our services around business domains, ensuring that our software models accurately reflect complex business realities. This approach enhances communication between technical and non-technical teams, promotes a deep understanding of the domain, and leads to more maintainable and scalable systems.

- **Event Sourcing**: We implement event sourcing to record all changes to the application state as a sequence of immutable events. This practice allows us to maintain a complete and auditable history of state changes, enabling features like time travel debugging, audit logs, and the ability to rebuild system state by replaying events.

- **Command Query Responsibility Segregation (CQRS)**: By separating read and write operations into distinct models, CQRS enables us to optimize each for its specific use case. This separation improves performance, scalability, and security, as we can tailor the read model for query efficiency and the write model for transactional integrity without compromise.

## How We Work

Our engineering culture is centered around best practices and methodologies that enhance productivity, collaboration, and code quality.

- **Trunk-Based Development**: We adopt trunk-based development to streamline our integration process. This practice involves developers committing small, frequent changes and deploying those directly out of a Pull Request in a GitOps way into lower environments and production, minimizing merge conflicts and facilitating continuous integration and delivery. It accelerates the delivery of features and fixes, allowing us to respond quickly to user needs and market changes.

- **Functional Programming**: Particularly on the backend, we leverage functional programming paradigms to write clean, modular, and testable code. Functional programming promotes immutability and pure functions, reducing side effects and making our codebase more predictable and easier to maintain. This approach enhances the reliability and scalability of our systems.

- **Multidisciplinary Teams**: We believe that the best solutions emerge from the collaboration of diverse skill sets and perspectives. Our teams are multidisciplinary, bringing together experts from engineering, design, product and all other fields relevant for a certain project. This cross-functional approach fosters innovation by combining technical expertise with user-centric design and strategic insights. It ensures that all aspects of a problem are considered, leading to holistic and effective solutions. By working collaboratively, we can iterate quickly, learn from each other, and deliver products that truly meet the needs of our users.

### Our Approach to Development

At JUCR, we believe in a structured and framework-based approach to software development, which enhances the maturity of our codebase and aims to create a seamless development experience for our engineers. This philosophy is embodied in our projects like **lightning-ts** and **lightning-rs**, collections of concepts that align with our vision of effective software architecture in TypeScript and Rust, respectively.

**lightning-ts** and **lightning-rs** provide guiding frameworks with recommendations on how to build and architect high-quality applications. They include techniques, best practices, architectural patterns, and guidelines sourced from various proven methodologies, all tailored to meet our specific needs. The core emphasis of these projects is to elevate our development processes by offering a comprehensive guide for our engineers.

The patterns and principles presented in **lightning-ts** and **lightning-rs** are framework-agnostic, ensuring that our core packages are not tied to any specific technologies. This flexibility allows teams to adopt these recommendations without being constrained by implementation details, promoting a wider adoption across different projects within JUCR.

We also leverage **reusable GitHub Actions workflows** to streamline our continuous integration and continuous delivery (CI/CD) pipelines. By creating modular and reusable workflows, we reduce duplication and enforce consistent standards across projects. This approach not only accelerates the development cycle but also ensures that all projects benefit from shared best practices, such as automated testing, linting, and security checks.

While we provide these frameworks and workflows as recommendations rather than strict rules, we encourage our teams to consider them when developing production applications. Each project comes with unique requirements, so any pattern or principle can be adjusted or omitted as necessary to best fit the project's context. 

By leveraging the recommendations in **lightning-ts**, **lightning-rs**, and our reusable GitHub Actions workflows, we aim to achieve several core benefits:

- **Clean Architecture**: A well-defined structure facilitates understanding and navigation of the codebase, making it easier for new team members to onboard and contribute.

- **Easy Maintenance**: Following established patterns leads to more maintainable code, reducing technical debt and allowing for smoother updates and changes over time.

- **Seamless Extension**: The architecture is designed to support extensibility, enabling teams to add new features and functionalities without disrupting existing systems.

- **Improved Automation**: Reusable workflows for GitHub Actions ensure that processes like CI/CD are automated and standardized, reducing manual errors and increasing development velocity.

- **Low Leadtime**: Our CI/CD and review process allow us to push a PR to production in 7 minutes.


## Our Commitment to Quality and Innovation

At JUCR, we are committed to continuous improvement and innovation. We invest in research and development to stay at the forefront of technology and e-mobility solutions. Our team regularly participates in industry conferences, workshops, and training sessions to expand their skills and knowledge.

We also prioritize security and compliance, implementing robust security measures and adhering to industry standards and regulations to protect our users and data.

# Open Source at JUCR

We are avid supporters of the open-source community. JUCR extensively utilizes open-source libraries and tools, which are integral to our technology stack. In the spirit of giving back, we actively contribute to open-source projects and encourage our engineers to dedicate a portion of their work time to contribute to these projects. This not only helps improve the tools we rely on but also fosters innovation and collaboration within the community.

Our commitment to open source is reflected in several projects we have publicly launched:

- **[Pathfinder](https://github.com/jucr-io/pathfinder)**: Pathfinder is a Kubernetes-native relay that bridges an asynchronous message broker like Apache Kafka with the Apollo Router. It includes adapters for Kafka, Redis, and Apollo, and supports multiple serialization and deserialization formats such as Protobuf or JSON Schema, optionally even with connection to an external schema registry. Pathfinder simplifies the process of integrating event-driven architectures with GraphQL APIs, enhancing scalability and performance. It allows developers to build responsive applications that can handle real-time data streams efficiently.

- **[Firmware Controller](https://github.com/jucr-io/firmware-controller)**: This procedural macro simplifies the decoupling of interactions between components in a `no_std` environment, which is crucial for embedded systems programming where standard libraries are not available. Firmware Controller enables developers to write more modular and maintainable code by abstracting complex patterns and reducing boilerplate. It aids in building robust firmware for microcontrollers, enhancing the reliability of embedded systems.

- **[Modem Kick](https://github.com/jucr-io/modem-kick)**: Modem Kick is a systemd service that listens to ModemManager for registration state changes. It performs the necessary power operations to wake up a modem when the registration state returns back to normal. This tool is essential for maintaining reliable connectivity in devices that rely on modem communication, such as IoT devices and remote sensors. It ensures they can recover from network disruptions automatically, reducing downtime and maintenance efforts.

## Get Involved

We welcome contributions from the community. Whether you're interested in collaborating on our open-source projects, have ideas for new features, or want to report issues, we encourage you to get involved. Check out our repositories on GitHub, and feel free to reach out to us through the provided channels.

## Join Our Team

If you're passionate about e-mobility, innovative technologies, and making a positive impact on the environment, consider joining our team. We offer exciting career opportunities in a dynamic and inclusive environment. Visit our [careers page](https://career.jucr.com) for current openings.
