# Elastic Agent and Ingest Manager

## Overview

* Setup Elastic Agent
* Ingest data

### Setup Elastic Agent

1. Download [Nginx sample log](https://github.com/sherry-ger/wwc-meetup/raw/master/Data/nginx.log).
2. Download Elastic Agent.

**MacOs**

```
curl -L -O https://artifacts.elastic.co/downloads/beats/elastic-agent/elastic-agent-7.9.1-darwin-x86_64.tar.gz
tar xzvf elastic-agent-7.9.1-darwin-x86_64.tar.gz
```
**Windows**

```
Download the Elastic Agent Windows zip file from the [downloads page](https://www.elastic.co/downloads/elastic-agent).
Extract the contents of the zip file into C:\Program Files.
Rename the elastic-agent-<version>-windows directory to Elastic-Agent.
```

3. Launch Elastic Cloud Kibana

<img src="/Labs-ElasticCloud/images/cloud8.png" alt="virtual_class" width="620" height="420">

4. Go to Management > Ingest Manager.

<img src="/Labs-ElasticCloud/images/ingest1.png" alt="virtual_class" width="250" height="1000">

5. In the Ingest Manager, click the Integrations tab and use the search bar to find the Nginx integration.. 

<img src="/Labs-ElasticCloud/images/ingest2.png" alt="virtual_class" width="400" height="240">

<img src="/Labs-ElasticCloud/images/ingest3.png" alt="virtual_class" width="600" height="300">

6. Click the Nginx integration to see more details about it, and then click Add Nginx. 

<img src="/Labs-ElasticCloud/images/ingest4.png" alt="virtual_class" width="720" height="270">

7. On the Add Nginx integration page, click the default agent configuration to select it, then scroll down to inspect or change the default settings.

<img src="/Labs-ElasticCloud/images/ingest5.png" alt="virtual_class" width="725" height="360">

8. Click the down arrow next to Collect logs from Nginx instances and change the Paths field. 

<img src="/Labs-ElasticCloud/images/ingest6.png" alt="virtual_class" width="440" height="480">

9. In the Nginx access logs path, please provide the Nginx log location to our download from step 1. For me, it is at

`/Users/sherryger/SherryDocuments/wwc-meetup/Data/*.log`

<img src="/Labs-ElasticCloud/images/ingest7.png" alt="virtual_class" width="420" height="540">

10. When you’re done, click Save integration.

11. Click on the Fleet tab.

<img src="/Labs-ElasticCloud/images/ingest8.png" alt="virtual_class" width="730" height="270">

12. Enable Fleet by clicking on Create user and enable Fleet.

<img src="/Labs-ElasticCloud/images/ingest9.png" alt="virtual_class" width="610" height="275">

13. On the Fleet tab, click Add agent and complete the steps under Enroll with Fleet. Please skip step 1 and step2. We have completed them earlier. Please find the OS your are using and follow the steps to start the agent. Please note, copy and paste the commands into an editor and run them one at a time.

<img src="/Labs-ElasticCloud/images/ingest10.png" alt="virtual_class" width="430" height="640">

That is it!  Let's take a look at our data in Kibana dashboards.

<img src="/Labs-ElasticCloud/images/ingest11.png" alt="virtual_class" width="935" height="535">
