# IOC Dashboard For Splunk
This dashboard is designed to identify IOC matches from a lookup file.

## Requirements & Recommendations:
### Requirements:
- **Splunk Common Information Model (CIM)**
  - https://splunkbase.splunk.com/app/1621
- **Splunk Add-on for Sysmon**
  - https://splunkbase.splunk.com/app/5709
- **TA For Zeek**
  - https://splunkbase.splunk.com/app/5466
- **Hashes_Datamodel.json** must be configured and installed (Datamodel ID: Sysmon_Hashes)
- **Zeek_Datamodel.json** must be configured and installed (Datamodel ID: Zeek_IP_DNS)
- **IP_iocs.csv** Lookup File (Data Needed)
- **Domain_iocs.csv** Lookup File (Data Needed)
- **URL_iocs.csv** Lookup File (Data Needed)
- **MD5_iocs.csv** Lookup File (Data Needed)
- **SHA256_iocs.csv** Lookup File (Data Needed)
- **IOC Dashboard v7-1.xml** is the source code for the dashboard
 
### Recommendations: 
- **Splunk App For Lookup File Editing**
  - https://splunkbase.splunk.com/app/1724

## Current Version Notes:
- Version 7 dashboard panels now utilize a flow of operations to limit concurrent searches.

## Other Notes:
- It is recommended that you pull your IOCs from Crowdstrike. The fields in the CSV are designed to match.
- The _Hashes_Datamodel.json_ is the same datamodel used for the _Suricata Alert Dashboard For Splunk_
