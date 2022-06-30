# Kibana Dashboards

Creating your first set of dashboards for Kibana can have quite the learning curve! Hopefully these can help you get started with an initial set of visualizations focused on finding anomalies.

## Zeek

Zeek is an open-source network security monitoring tool that does a really good job at session and protocol analysis. To find out more about Zeek, check out: [https://zeek.org/](https://zeek.org/)

Current supported protocols/logs: CONN (conn.log), DNS, HTTP, TLS (SSL), SMB, RDP, NTLM, Files, and Weird (weird.log).

All the dashboards are organized with the following flow:
- High-level connection info including IPs and ports
- Protocol specific information that may be helpful for finding anomalies
- All dashboards end with a saved search so you can expand the full records for investigation

All the dashboards have associated screenshots in the Images folder so you can check them out. 

## Importing Steps (Elastic v7.x)

1. Navigate to Stack Management in Kibana via the left-navigation menu

2. Click on "Saved Objects" (Under Kibana)

3. In the top-right there is an "Import" button

4. Select the .ndjson file and Import!

This includes the dashboards, associated visualizations, and an index pattern for "filebeat-*"

**Note:** If you are using another index pattern for your zeek data, you will have to do some editing on the .ndjson file for the index pattern and field names to be associated properly.