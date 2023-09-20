---
title: 10. Systems Behind Interactions
weight: 110
---

## Intro to Splunk Dashboard

What is Splunk? Splunk is a visual representation of machine data (or unstructured data). We talk more on unstructured data later in this section but for not we will focus on search. Splunk searches, monitors and analyzes data and allows us to create alerts, reports and dashboards. We can use regular expressions and Structure Query Language (SQL) like syntax to collect data and view results in a web-based interface using Search Processing Language (SPL). Splunk along with other related software is an observability tool, which means it allows logging, monitoring and application performance management features that allow us to debug and analyze application data. Monitoring is one of the most important tools that an information Technology (IT) team can use. Additionally, monitoring tools allow us to collect host metrics, collect data about the application and send notifications if the application becomes unresponsive. As technical analysts, we will likely interact with the following teams who get notified or create the alerts that notify us.  

1. **Tier 2, Tier 3 Support** - this team is on the front line with clients and may need a hand from other teams (DevOps, SRE )for more in-depth technical issues.
2. **Development** - As we become subject matter experts (SMEs) we may be pulled into meetings with the development team to help answer questions about the application
3. **DevOps** - since DevOps typically owns the delivery of software, they will be interested to know how well it is performing for end users.

## Why are we monitoring

Service Level Agreement (SLA), Service Level Objectives (SLO)and Service Level Indicators (SLI) are different concepts we use to describe a business level partnership agreement and helps to measure the agreement to ensure we have met the expectations. SLAs are business-level agreements that define the service availability for a customer and the penalties for not reaching the availability (e.g. 99.9999% availability). 

SLOs are agreements on how often the SLIs must be met and provide a target value or range of values for a service level that is measured by an SLI. SLIs are metrics over time which inform about the health of a SLA & SLO agreement. 

Crafting an SLA requires business and legal teams to work together to pick appropriate consequences and penalties for a breach of an SLA. It is wise to be conservative in what we advertise to users since the larger the user base and expectation, the harder it will be to modify or remove an SLA. Additionally, a SLOs allows us to detect and correct issues before they are reported which make them critically important to support the SLA and ensure we have reliability baked into our applications and services.  

## Introduction to Splunk

Splunk Application Performance Management (APM) features four areas of monitoring. These areas allow us to monitor SLIs and alert them when they reach a critical level. APM features the below sections:  

1. No Sample Distributed Tracing 
2. Real Time Monitoring 
3. Performance Optimization 
4. Troubleshoot Latencies and Errors 

**No Sample Distributed Tracing,** collects and analyzes data from every services that you have connected to Splunk

**Real Time Monitoring**, with built-in dashboards that automatically capture metrics for each service in an application. These dashboards can be used to create dynamic alerts based on changes and anomalies. 

**Performance Optimization**, allows us to identify bottlenecks and optimize our applications through code-level, service instances and database queries.   

**Troubleshoot Latencies and Errors**, let us investigate the root cause of problems in our application using APM’s features like Service Map, Tag, Spotlight and Always On Profiling.  

## Splunk Infrastructure Monitoring

Splunk Infrastructure Monitoring is part of Splunk Observability Cloud. It provides a simple and comprehensive platform to monitor and troubleshoot our infrastructure and applications. We can leverage the metrics from any source at scale and detect issues in real-time across deployments.
