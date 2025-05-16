# devops-learning-path
A collaborative guide for learning DevOps concepts and tools

# DevOps Learning Journey: Concepts and Tools

This document outlines a comprehensive list of concepts and tools valuable for becoming a proficient DevOps engineer, grouped into logical categories for structured learning.

## Foundational Infrastructure & Networking

* **DNS:** Understanding domain name resolution and managing DNS servers.
    * `Bind9`
    * `dnsmasq`
* **Networking Fundamentals:** (Implicit but essential) TCP/IP, Ports, Subnets, Routing.
* **NTP:** Time synchronization protocol.
    * `chrony`
    * `ntpd`
* **NFS:** Network File System for shared storage.
    * `FreeNAS`
    * `OpenNFS`

## Operating Systems & Scripting

* **Linux/Unix Fundamentals:** Command line proficiency, process management, file systems.
* **Scripting Languages:** (Essential for automation)
    * Bash
    * Python
    * (Potentially others like Ruby, Go)

## Configuration Management & Infrastructure as Code (IaC)

* **Configuration Management:** Automating system configuration and desired state.
    * `Ansible`
    * `AnsibleTower` (or AWX)
* **Infrastructure as Code (IaC):** Provisioning and managing infrastructure through code.
    * `Terraform`
    * (Cloud-specific IaC tools like CloudFormation, ARM Templates/Bicep - recommended based on cloud focus)

## Containerization & Orchestration

* **Containerization:** Packaging applications and dependencies into containers.
    * `Docker`
* **Container Orchestration:** Managing and automating the deployment, scaling, and operation of containerized applications.
    * `Kubernetes (K8s)`

## Databases (SQL & NoSQL)

* **Database Concepts:**
    * Querying
    * Optimization
    * Partitioning
    * Read Replicas
    * Sharding
    * Archival and Backup
* **SQL RDBMS:** Relational Database Management Systems.
    * `MySQL`
    * `PostgreSQL`
    * `Galera Cluster` (for MySQL High Availability)
* **NoSQL:** Non-relational Databases.
    * `Cassandra`
    * `MongoDB`
    * `Apache CouchDB`

## CI/CD (Continuous Integration / Continuous Delivery)

* **CI/CD Principles:** Understanding the workflows and benefits of automated build, test, and deployment pipelines.
* **CI/CD Tools:**
    * `Jenkins`
    * `Github Actions`
    * (Others like GitLab CI, CircleCI, Travis CI, Azure DevOps Pipelines, AWS CodePipeline/CodeBuild)

## Monitoring, Logging, & Observability

* **Monitoring Concepts:** Instrumentation, Metrics, Alerts.
* **Infrastructure Monitoring:** Monitoring host and service health/performance.
    * `Zabbix`
    * `Prometheus`
* **APM Monitoring:** Application Performance Monitoring.
    * `GlowRoot` [Java]
    * `Java Melody`
    * `Apache Skywalking`
* **Telemetry:** Collecting data about your system's behavior.
    * `OTEL` (OpenTelemetry) [related to ApacheSkywalking]
* **Dashboarding:** Visualizing metrics and logs.
    * `Grafana`
    * `Cronograf` [TICK Stack]
* **Log Monitoring & Analysis:** Collecting, aggregating, and analyzing logs.
    * `LogWatch`
    * `Greylog`
    * `Elasticsearch / ELK Stack` (often used for log analysis along with Kibana)
    * `Solr` (also used for searching, including logs)

## Security & Access (DevSecOps)

* **DevSecOps Principles:** Integrating security throughout the development lifecycle ("Shift Left").
* **Firewalls:** Host-based firewall management.
    * `UFW`
    * `Firewalld`
* **Jumpbox:** Secure bastion hosts for accessing internal networks.
    * `JumpServer`
* **Security Monitoring:** (Related to Jumpbox) Perimeter Monitoring, general Security Monitoring concepts.
* **LDAP:** Directory services for centralized authentication/authorization.
    * `ApacheDS`
    * `389Directory Server`
* **VPN:** Virtual Private Network for secure remote access.
    * `OpenVPN` [Client/Server]
* **SIEM:** Security Information and Event Management (often involves log analysis).
    * `osquery` (Endpoint visibility)
* **Vulnerability Scanning:** (DevSecOps practice) Tools for scanning code, dependencies, and infrastructure.
* **Secrets Management:** (DevSecOps practice) Securely storing and managing secrets.

## High Availability & Clustering

* **Clustering Technologies:**
    * `corosync`
    * `keepalived`
    * `pacemaker`
    * `heartbeat`
* **Concepts:** Failover, Redundancy, Quorum.

## Job Scheduling & Data Processing

* **Time Based Job Scheduling:** Executing tasks at specific times or intervals.
    * `AT`
    * `anacron`
    * `Crond`
    * `InCrond`
    * `Cronicle`
    * `Pentaho` (Often used for ETL/ELT jobs)
* **Event Based Job Scheduling:** Triggering tasks based on specific events.
    * `OpenFAAS` (Serverless functions can be event-driven)
* **ETL/ELT:** (Concept) Extract, Transform, Load or Extract, Load, Transform data pipelines.
    * Job Monitoring (Monitoring ETL/ELT jobs)

## Messaging & Streaming

* **Message Queues:** Enabling asynchronous communication between applications.
    * `ActiveMQ`
    * `RabbitMQ`
* **Streaming:** Processing continuous streams of data.
    * `Kafka`
* **General Messaging:**
    * Email Server and Clients
    * Messaging Server [`Openfire`] and Client

## Other Infrastructure Components

* **State Management / Distributed Coordination:**
    * `Zookeeper`
* **Search Services:**
    * `ElasticSearch` (Part of ELK)
    * `Solr`
    * `Sphinx`
* **Caching:** Improving performance by storing frequently accessed data in memory.
    * `Redis`
    * `MemCache`

## Application Runtimes & Management

* **Application Servers:**
    * `Tomcat9/10`
    * `Jetty`
    * `JBOSS/Pyara/GlassFish`
* **Application Monitoring & Management:**
    * `JMX` (Java Management Extensions)
    * Custom Metrics [JSON Parsing/Monitoring]

## Web Technologies

* **Web Servers:** Serving web content.
    * `Apache2`
    * `NGINX`
    * `Caddy`
    * `Openlitespeed`
    * `lighttpd`
    * `thttpd`
* **Proxies & Load Balancers:** Distributing traffic and providing a single entry point.
    * `HA Proxy`
    * `NGINX` (also functions as a proxy/LB)
    * `Traefik`
    * `LVS` (Linux Virtual Server)
    * `Zeevnet` (Likely referring to technologies/concepts related to load balancing)
* **API Gateway:** Managing, securing, and routing API traffic.
    * `Apache APISIX`

## Specialized Areas

* **CMS (Content Management Systems):**
    * `Wp` (WordPress)
    * `Joomla`
    * `Drupal`
* **Chaos Engineering:** Intentionally injecting failures to test system resilience. (No specific tools listed in your original list, but tools like Gremlin or Chaos Monkey are examples).
* **Cloud Computing:** (Crucial, pick a provider to focus on) AWS, GCP, Azure.

## General DevOps Concepts

* **Monitoring:**
    * Instrumentation
    * Metrics
    * Alerts
* **Deploy:**
    * Install
    * Upgrade
    * Configure
    * Backup
    * DR (Disaster Recovery)
