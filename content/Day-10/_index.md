---
title: 10. Systems Behind Interactions
weight: 110
---

## Intro to Splunk 

What is Splunk? Splunk is a visual representation of machine data. Machine data is also known as unstructured data. We'll talk more about unstructured data later in this section, but for now, we will focus on Splunk search. Splunk searches, monitors, and analyzes data and allows us to create alerts, reports, and dashboards. 

We can use regular expressions and Structured Query Language (SQL)-like syntax to collect data and view results in a web-based interface using Splunk's Search Processing Language (SPL). Splunk, along with other related software, is an observability tool, which means it has logging, monitoring, and application performance management features that allow us to debug and analyze application data. 

Monitoring is one of the most important tools that an information technology (IT) team can use. It allows the IT team to be proactive instead of reactive to system outages and issues. Additionally, monitoring tools allow us to collect host metrics, data about the application, and send notifications if the application becomes unresponsive. As technical analysts, we will likely be Tier 1 support, and we may interact with the following teams who also get notified, or they may even create some of the alerts that notify us.

1. **Tier 2, Tier 3 Support** - this team is also a front-line team that interacts with clients or customers. They may need a hand additional support from other teams like the DevOps Engineer and Site Reliability Engineer (SRE) for more in-depth technical issues.
2. **Development** - As we become subject matter experts (SMEs) we may be pulled into meetings with the development team that is responsible for application. We may be asked to help clarify the problem or solution for an application
3. **DevOps** - since DevOps typically owns the delivery of software, they will be interested to know how well it is performing for end users. Given time, Technical Analyst will hold intimate knowledge of a system which allows them gain insights that can be critical to application enhancements.
   
## Splunk Infrastructure Monitoring

Splunk Infrastructure Monitoring is part of Splunk Observability Cloud. It provides a simple but comprehensive platform to monitor and troubleshoot system infrastructure and applications. We can leverage the metrics from any source connected to Splunk at scale and detect issues in real-time across the organization. 

These observability tools provide insight into the machines, systems, and applications in production environments, allowing members in the organization to create response teams, policies, system backups, disaster recovery, and business continuity plans. Additionally, having an observability tool creates a data-driven decision culture, enabling teams to create dashboards specific to their team monitoring needs and aligning these metrics with organizational goals and Service Level Agreements (SLAs).

## Why are we monitoring

**Service Level Agreement (SLA)**, **Service Level Objectives (SLO)**, and **Service Level Indicators (SLI)** are different concepts we use to describe a business-level agreement and help to measure the agreement between a business and its end-users. Monitoring these three (3) areas ensures we have met the expectations of our clients and partners. **SLAs** are business-level agreements that define the service availability of a system for a customer and the penalties for not reaching the availability (e.g. 99.9999% availability). **SLOs** are agreements on how often the SLIs must be met and provide a target value or range of values for a service level that is measured by an SLI. SLIs are metrics used over time that inform us about the health of a given SLA & SLO agreement.

Crafting an SLA requires business and legal teams to work together to pick appropriate consequences and penalties for a breach marked SLA. It is wise to be conservative in what we advertise to users since the larger the user base and expectations, the harder it will be to modify or remove an SLA. Additionally, SLOs allow us to detect and correct issues before they are reported, which makes them critically important to support the SLA and ensure we have reliability baked into our applications and services.

## Introduction to Splunk

Splunk Application Performance Management (APM) features four areas of monitoring. These areas allow us to monitor SLIs, notification and alerts when they reach a low, medium or high (critical) levels. APM features the below sections:  

1. No Sample Distributed Tracing 
2. Real Time Monitoring 
3. Performance Optimization 
4. Troubleshoot Latencies and Errors 

**No Sample Distributed Tracing** collects and analyzes data from every service that you have connected to Splunk. This includes web servers, databases, and API requests. This information is collected and forwarded to Splunk search head for further analysis. We can also pull system metrics like CPU, memory utilization, and storage into a dashboard for a review of system available resources.

**Real-Time Monitoring** with built-in dashboards that automatically capture metrics for each service in an application. These dashboards can be used to create dynamic alerts based on changes and anomalies in the system. For example, if we used Real-Time Monitoring (RTM) in a fraud detection service for user account services at Mastercard, this service would monitor card transactions in real time and detect anomalies like purchases in California in rapid succession. This service would be able to detect, capture, and prevent fraud on a customer's transaction as they are happening.

**Performance Optimization** allows us to identify bottlenecks and optimize our applications through code-level, service instances, and database queries. This means we can scale our applications proactively instead of reactively to reported issues by customers. Performance optimization may require isolated alerts in a golden dashboard. A golden dashboard is a dashboard known to SREs as monitoring of latency, traffic, errors, and saturation in a system. These can be separate from SLAs and logging metrics to keep the dashboard focused on key resources in the organization. Latency in a system or lack refers to a delay between a request. For example, when we type a website into the web browser, the time between hitting enter on our keyboard and the page showing up on the screen is the latency time.

Traffic in performance is directly related to how many client machines are sending requests to the web server. In other words, how many people are coming to the site at any given time. Errors are issues that happen mostly between system communications, like the 404-https status code we get when we are requesting a resource that is no longer available or a 500-status code if the web server is down. Saturation is a reference to the Inputs and Outputs, available memory, and system load under stress or heavy load. For example, if 100,000 client machines are trying to access the web server or database, saturation should inform us in a proactive alert before we reach total failure in a system.

**Troubleshoot Latencies and Errors** allows us to investigate the root cause of problems in our application using APM's features and services Map, Tag, Spotlight, and Always On Profiling. When these features are enabled, we can monitor, report, and alert on systems and determine the health of our applications and services.



