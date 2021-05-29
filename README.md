# AWS Transfer for SFTP

This sample code demonstrates how to configure per-user logical directory configurations as part of a custom identity provider for use with the 
AWS Transfer for SFTP service.  To see the sample in action you can deploy the code into your AWS account now using one of the buttons below or you
can clone this repository and explore the code for yourself.

This repository contains the following files:
```
├── README.md
├── cloudformation
│   ├── main.yaml               <-- CloudFormation to deploy S3 buckets, an SFTP server, and identity provider
│   ├── sftp_idp.yaml           <-- CloudFormation to provision custom identity provider
│   └── sftp_server.yaml        <-- CloudFormation to provision Transfer for SFTP server
└── src
    ├── authorizor
    │   └── lambda.js           <-- custom identity provider, responsible for configuring logical directories
    └── datagen
        └── lambda_function.py  <-- custom resource to generate sample data, part of cloudformation
```

