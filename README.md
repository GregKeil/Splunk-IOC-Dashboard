# IOC Dashboard For Splunk
This dashboard is designed to identify IOC matches from a lookup file.

## Notes:
- For proper usage of this dashboard, datamodels must be established for Sysmon and Zeek.
- A lookup table containing the IOC information must also be established.
- In order to ensure that the datamodels stay up to date even when the analyst only looks at previously stored information, scheduled reports must be created.

## Requirements & Recommendations:
### Requirements:
- **Splunk Common Information Model (CIM)**
  - https://splunkbase.splunk.com/app/1621
- **Splunk Add-on for Sysmon**
  - https://splunkbase.splunk.com/app/5709
- **TA For Zeek**
  - https://splunkbase.splunk.com/app/5466
- **Hashes.json** (Datamodel) must be configured and installed
- **Zeek.json** (Datamodel) must be configured and installed
- **IP_iocs.csv** Lookup File
- **Domain_iocs.csv** Lookup File
- **URL_iocs.csv** Lookup File
- **MD5_iocs.csv** Lookup File
- **SHA256_iocs.csv** Lookup File
 
### Recommendations: 
- **Splunk App For Lookup File Editing**
  - https://splunkbase.splunk.com/app/1724

## Current Version Notes:
- Version 7 dashboard panels now utilize a flow of operations to limit concurrent searches.

## Other Notes:
- It is recommended that you pull your IOCs from Crowdstrike. The fields in the CSV are designed to match.
