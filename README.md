**Motivation** - Feed Custom Threat Intelligence to AWS GuardDuty

**Details?** - Malicious IP list is periodically fetched from https://www.abuseipdb.com/
           and fed as custom IP list to GuardDuty.

**Architecture**
![GuardDuty-CustomTI](https://user-images.githubusercontent.com/16767739/149082033-70f1c61d-e01c-4223-8edb-a32754771645.png)

**ToDo** - Combine the two yaml templates to one - Needs defining a custom resource in CloudFormation and run
       a Lambda function to create the object in S3 bucket for the Resource 'AWS::GuardDuty::ThreatIntelSet'
       to access during stack creation.
