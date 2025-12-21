**Centralized Windows Event Log Analysis with Splunk**



This example will show how Windows Security logs can be collected, centralized, and analyzed with Splunk.



It was to grasp how alerts are passed from an endpoint to a SIEM, and how events for authentication can be queried after being centralized.



**Scenario**



For Windows systems, it logs Security events, including logon successes or failures.



Unlike analyzing local events, logs are submitted to a central Splunk server for analysis and monitoring.



**Environment**

\- Windows VM (Log Source)

\- Windows Event Log of Security Events

\- Splunk Universal Forwarder

\- Linux VM (SIEM server)

\- Splunk Enterprise



**"Network communication"**



\- The logs are transmitted to Splunk using TCP port 9997

Even so, the following actions

\- Setup and implemented Splunk Enterprise on a Linux environment

– Installed the Splunk Universal Forwarder on Windows.



\- Forwarder was configured to retrieve the Windows Security events



\- Sent logs to the Splunk server for indexing

\- Evaluated ingestion and events related to authentication using Splunk searches



**Example analysis**



These types of events were investigated:

\- Successful logons (EventID 4624)



\- Logon failures (Event ID 4625)



**Searches were employed in the following ways:**



Comparison of successful vs failed logins - Detect accounts that create auth events – Instead of analyzing event time series on the endpoint, do the analysis at the central server.

Notes "This is a beginner project, and it emphasizes understanding the fundamentals of a SIEM system and the flow of logs, **and it is not about making complex alerts and charts In-depth**.

screen captures are included within the repository.

