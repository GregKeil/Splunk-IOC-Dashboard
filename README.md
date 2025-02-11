# IOC Dashboard For Splunk
This suite of dashboards is designed to identify IOC matches from lookup files.

## Requirements & Recommendations:
### Requirements:
- **Splunk Common Information Model (CIM)**
  - https://splunkbase.splunk.com/app/1621
- **TA For Zeek**
  - https://splunkbase.splunk.com/app/5466
 
### Recommendations: 
- **Splunk App For Lookup File Editing**
  - https://splunkbase.splunk.com/app/1724

## Other Notes:
- It is recommended that you pull your IOCs from Crowdstrike. The fields in the CSV are designed to match.
- The _Hashes_Datamodel.json_ is the same datamodel used for the _Suricata Alert Dashboard For Splunk_
