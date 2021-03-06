---
title: "OVH"
date: 2019-03-03T16:39:46+01:00
draft: false
slug: ovh
---

<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
<!-- providers/dns/ovh/ovh.toml -->
<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->


Configuration for [OVH](https://www.ovh.com/).


<!--more-->

- Code: `ovh`

{{% notice note %}}
_Please contribute by adding a CLI example._
{{% /notice %}}




## Credentials

| Environment Variable Name | Description |
|-----------------------|-------------|
| `OVH_APPLICATION_KEY` | Application key |
| `OVH_APPLICATION_SECRET` | Application secret |
| `OVH_CONSUMER_KEY` | Consumer key |
| `OVH_ENDPOINT` | Endpoint URL (ovh-eu or ovh-ca) |


## Additional Configuration

| Environment Variable Name | Description |
|--------------------------------|-------------|
| `OVH_HTTP_TIMEOUT` | API request timeout |
| `OVH_POLLING_INTERVAL` | Time between DNS propagation check |
| `OVH_PROPAGATION_TIMEOUT` | Maximum waiting time for DNS propagation |
| `OVH_TTL` | The TTL of the TXT record used for the DNS challenge |




## More information

- [API documentation](https://eu.api.ovh.com/)
- [Go client](https://github.com/ovh/go-ovh)

<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
<!-- providers/dns/ovh/ovh.toml -->
<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
