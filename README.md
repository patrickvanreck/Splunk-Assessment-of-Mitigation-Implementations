# Splunk Assessment of Mitigation Implementations

Mitigation implementations have not traditionally been evaluated or prioritized. NSA Information Assurance recommends mitigation strategies but there are few methods to validate proper implementation and prioritize fixes. The SAMI application was developed to monitor the degree to which specific aspects of the [NSA Information Assurance](https://www.iad.gov/) [top 10 mitigation strategies](https://www.iad.gov/iad/library/ia-guidance/iads-top-10-information-assurance-mitigation-strategies.cfm) have been deployed on Windows endpoints. It monitors data related to the implementation of specific mitigations and returns prioritized recommendations to more completely implement those recommendations. The application can be used to determine a network’s mitigation implementation status and can be monitored over time to demonstrate improvements and identify changes that negatively impact mitigations.

SAMI evaluates several metrics:
* Modern Operating System (MOS)
* Anti-Virus File Reputation Service (AVFRS)
* Host Intrusion Prevention System (HIPS)
* Application Whitelisting (AW)
* Anti-Exploitation (AE)
* Pass-the-Hash (PtH) 

The application aims to make automated measurement of mitigations both common and understandable. More specifically, the goals for SAMI are to:
* Establish the importance of measuring mitigations;
* Jumpstart community discussion on the topic; 
* Motivate vendors to support and build upon the capabilities;
* Establish the concept and process of scoring mitigations as part of vulnerability risk scoring

## Components

There are two main components:
* [SAMI](./SAMI) - Main application.
* [SAMI-TA](./SAMI-TA) - Addon for data collection pieces of the SAMI application.

These components are available as [Splunk](https://www.splunk.com/) applications and can be downloaded from [Splunkbase](https://splunkbase.splunk.com/):
* [SAMI - Splunk Assessment of Mitigation Implementations](https://splunkbase.splunk.com/app/3114/)
* [Technical Addon for SAMI Application (TA-SAMI)](https://splunkbase.splunk.com/app/3115/)

The source code for the binary components ([ae.exe](https://github.com/iadgov/LOCKLEVEL/tree/master/LL_AE) and [av.exe](https://github.com/iadgov/LOCKLEVEL/tree/master/LL_AV)) in SAMI-TA are available in the [LOCKLEVEL](https://github.com/iadgov/LOCKLEVEL) repository.

## Documentation

Documentation available for SAMI:
* User instruction manual:
    * [Download PDF](https://github.com/iadgov/Splunk-Assessment-of-Mitigation-Implementations/raw/master/SAMI_User_Instruction_Manual.pdf)
    * [View PDF on GitHub](https://github.com/iadgov/Splunk-Assessment-of-Mitigation-Implementations/blob/master/SAMI_User_Instruction_Manual.pdf)
* Business logic 
    * [Download Excel file](https://github.com/iadgov/Splunk-Assessment-of-Mitigation-Implementations/raw/master/SAMI_Business_Logic.xlsx)
    
A session about SAMI was given at [Splunk .conf2015](https://conf.splunk.com/speakers/2015.html):
* [Download video](https://conf.splunk.com/session/2015/recordings/2015-splunk-191.mp4)
* [Download slides](https://conf.splunk.com/session/2015/conf2015_sami_final_150908.pdf)

## License
See [LICENSE](./LICENSE.md).

## Disclaimer
See [DISCLAIMER](./DISCLAIMER.md).

