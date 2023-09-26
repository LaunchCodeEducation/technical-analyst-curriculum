---
title: 11. Splunk Components 
weight: 111
---

## System Architecture

There are three (3) main components of Splunk System Architecture Forwarders, Indexers and Search Heads. A Splunk Enterprise component is a Splunk Enterprise instance that performs a specialized task, like indexing data. There are several types of components that match the types of tasks in a deployment and they fall into two broad categories; Processing and Management Components. 

**Process components** handle data while **Management components** support  activities of the processing components. There are three types of processing components 

**Forwarders, **ingest raw data and forwards the data to another component such as another Forwarder or an indexer** ** 

**Indexers, **index and store data but they can also search data. They usually reside on a dedicated machine. They can be independent or in clusters (peer nodes or index clusters). A cluster is a physical grouping of machines in a collection in a particular region. 

**Search** **heads**, where Technical Analysts spend most of our time;**  **manage searches. They handle search requests from users and distribute the requests across indexers, which search their local data. They can be independent or in a search cluster or pool.  They help us to consolidate the results from all of the indexers and serve the results to the users. The search head provides the user with dashboards, reports and alerts that can be triggered given threshold.  They usually sit on dedicated Servers as independent search heads, or they can be in an indexer cluster, or search head pool. See the following diagram that shows how the Search Head represents a small enterprise with less than 100 users. 

![Splunk Search Head](/images/splunk-sh.png "Splunk Search Head Architecture View")
 
### Understanding the underlying systems Splunk is monitoring

**What is Unstructured Data?** This is data that is not in rows or columns. It is hard to read and manipulate the data and even harder to make sense of what might be in the dataset.  The following image shows an example of unstructured data from a Weblogic server. 

![Splunk Unstructured Data](/images/unstructured-data.png "How Unstructured Data Looks Without Using Splunk")

From the image above, it is really difficult to determine if there is a problem. We would need to look closely at all the output to determine a reported problem. Now, imagine we have one-hundred (100) servers and that we manage all with their own unique problem/error. This becomes a problem no one’s what to deal with on a daily basis. This is one of the problems Splunk solves by bringing structure to unstructured data. 

**What is Structured Data**? Structured data is the opposite of unstructured data and represents a clearer picture for us to read, work with and analyze data. It can be presented in rows and columns (tables or tabular data) and normally comes from a web server or event logs. Taking a look at the screenshot, you’ll notice a field **status : 200. **This is a common field that is an indicator that a webpage was returned to the user successfully. Other status codes like 400 series can be searched and presented to show us which pages did not return successfully. We can easily read a lot of the metadata about the request and response of the page using Splunk. 

{{% notice green "Protip" "rocket" %}}
**Note**: Http response codes tell us  if a particular request failed or was successful. This topic is outside of the scope of this book but should be reviewed at some point in your career journey.   
{{% /notice %}}

![Splunk Structured Data](/images/structured-data.png "How Structured Data Looks Using Splunk")

### Splunk Documentation & Community 

**Splunk Documentation** has two main platforms under the Splunk umbrella; Splunk Enterprise and Splunk Cloud. Based on the product we have installed the documentation will be different. Splunk Cloud provides insights for data at the petabyte-scale data analytics across a hybrid cloud solution. Splunk Enterprise allows us to search, analyze and visualize data for actionable insights from all of your data within the enterprise. 

### Splunk Community 

Start here