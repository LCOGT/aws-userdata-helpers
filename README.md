# AWS Userdata Helpers

Various helper scripts which can be run as part of an AWS Userdata Script when
an EC2 instance is launched to do some tasks.

Note that this repository is **PUBLIC**. Do not put any keys, passwords, or
other sensitive information into any script.

## Utilities

This section provides a brief overview of the scripts (utilities) which are
provided within this source code repository.

### route53-update-record

Update a single AWS Route53 DNS record with a new value. This script is
intended to be used to update an existing Route53 record to point to a new
machine as it is launched by an Autoscaling Group.

```
$ curl -fsSLO https://raw.githubusercontent.com/LCOGT/aws-userdata-helpers/master/route53-update-record
$ bash -x route53-update-record "$HOSTED_ZONE_ID" "$DNS_RECORD_NAME" "$DNS_RECORD_VALUE"
```

## License

This project is licensed under the MIT License. Please see the
[LICENSE](LICENSE) file for further details.
