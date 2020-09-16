# Elastic Agent and Ingest Manager

## Overview

* Setup Elastic Agent
* Ingest data

### Setup Elastic Agent

1. Download Elastic Agent.

**MacOs**

```
curl -L -O https://artifacts.elastic.co/downloads/beats/elastic-agent/elastic-agent-7.9.1-darwin-x86_64.tar.gz
tar xzvf elastic-agent-7.9.1-darwin-x86_64.tar.gz
```
**Windows**

  Download the Elastic Agent Windows zip file from the [downloads page](https://www.elastic.co/downloads/elastic-agent).
  Extract the contents of the zip file into C:\Program Files.
  Rename the elastic-agent-<version>-windows directory to Elastic-Agent.

2. Launch Elastic Cloud Kibana

<img src="/Labs-ElasticCloud/images/cloud8.png" alt="virtual_class" width="300" height="200">

3. Go to Management > Ingest Manager..

<img src="/Labs-ElasticCloud/images/ingest1.png" alt="virtual_class" width="700" height="300">

4. In Ingest Manager, click the Integrations tab and use the search bar to find the Nginx integration.. 

<img src="/Labs-ElasticCloud/images/ingest3.png" alt="virtual_class" width="400" height="150">

5. Click the Nginx integration to see more details about it, and then click Add Nginx. 

<img src="/Labs-ElasticCloud/images/ingest4.png" alt="virtual_class" width="400" height="150">

8.  On the Add Nginx integration page, click the default agent configuration to select it, then scroll down to inspect or change the default settings.

<img src="/Labs-ElasticCloud/images/ingest5.png" alt="virtual_class" width="400" height="150">

9.  Select the I/O Optimized template

<img src="/Labs-ElasticCloud/images/cloud4.png" alt="virtual_class" width="800" height="300">

10.  Click “Create deployment”.

11. Turn on <code>Machine Learning</code></strong> by clicking <strong><code>Enable</code></strong>.

<img src="/Labs-ElasticCloud/images/cloud6.png" alt="virtual_class" width="400" height="150">

13.  Click <code>Create deployment</code></strong>. Your cluster will begin to spin up.  It takes between 3 - 6 minutes to complete.

<img src="/Labs-ElasticCloud/images/img13.png" alt="virtual_class" width="300" height="50">

Please copy **the auto generated password** and down it.  \

<img src="/Labs-ElasticCloud/images/cloud7.png" alt="virtual_class" width="400" height="300">

14.  When the cluster is ready, click on launch next to the Kibana icon

<img src="/Labs-ElasticCloud/images/cloud8.png" alt="virtual_class" width="400" height="150">

That’s it for this lab! You have a deployment now ready to start ingesting and working with the data. 

