---
title: "Amazon Route 53"
date: 2019-03-03T16:39:46+01:00
draft: false
slug: route53
---

<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
<!-- providers/dns/route53/route53.toml -->
<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->


Configuration for [Amazon Route 53](https://aws.amazon.com/route53/).


<!--more-->

- Code: `route53`

{{% notice note %}}
_Please contribute by adding a CLI example._
{{% /notice %}}




## Credentials

| Environment Variable Name | Description |
|-----------------------|-------------|
| `AWS_ACCESS_KEY_ID` |  |
| `AWS_HOSTED_ZONE_ID` |  |
| `AWS_REGION` |  |
| `AWS_SECRET_ACCESS_KEY` |  |


## Additional Configuration

| Environment Variable Name | Description |
|--------------------------------|-------------|
| `AWS_POLLING_INTERVAL` | Time between DNS propagation check |
| `AWS_PROPAGATION_TIMEOUT` | Maximum waiting time for DNS propagation |
| `AWS_TTL` | The TTL of the TXT record used for the DNS challenge |

## Description

AWS Credentials are automatically detected in the following locations and prioritized in the following order:

1. Environment variables: `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `AWS_REGION`, [`AWS_SESSION_TOKEN`]
2. Shared credentials file (defaults to `~/.aws/credentials`)
3. Amazon EC2 IAM role

If `AWS_HOSTED_ZONE_ID` is not set, Lego tries to determine the correct public hosted zone via the FQDN.

See also: [configuring-sdk](https://github.com/aws/aws-sdk-go/wiki/configuring-sdk)

## Policy

The following AWS IAM policy document describes the permissions required for lego to complete the DNS challenge.

```json
{
   "Version": "2012-10-17",
   "Statement": [
       {
           "Sid": "",
           "Effect": "Allow",
           "Action": [
               "route53:GetChange",
               "route53:ChangeResourceRecordSets",
               "route53:ListResourceRecordSets"
           ],
           "Resource": [
               "arn:aws:route53:::hostedzone/*",
               "arn:aws:route53:::change/*"
           ]
       },
       {
           "Sid": "",
           "Effect": "Allow",
           "Action": "route53:ListHostedZonesByName",
           "Resource": "*"
       }
   ]
}
```




## More information

- [API documentation](https://docs.aws.amazon.com/Route53/latest/APIReference/API_Operations_Amazon_Route_53.html)
- [Go client](https://github.com/aws/aws-sdk-go/aws)

<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
<!-- providers/dns/route53/route53.toml -->
<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
