---
title: "Vultr"
date: 2019-03-03T16:39:46+01:00
draft: false
slug: vultr
---

<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
<!-- providers/dns/vultr/vultr.toml -->
<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->


Configuration for [Vultr](https://www.vultr.com/).


<!--more-->

- Code: `vultr`

{{% notice note %}}
_Please contribute by adding a CLI example._
{{% /notice %}}




## Credentials

| Environment Variable Name | Description |
|-----------------------|-------------|
| `VULTR_API_KEY` | API key |


## Additional Configuration

| Environment Variable Name | Description |
|--------------------------------|-------------|
| `VULTR_HTTP_TIMEOUT` | API request timeout |
| `VULTR_POLLING_INTERVAL` | Time between DNS propagation check |
| `VULTR_PROPAGATION_TIMEOUT` | Maximum waiting time for DNS propagation |
| `VULTR_TTL` | The TTL of the TXT record used for the DNS challenge |




## More information

- [API documentation](https://www.vultr.com/api/#dns)
- [Go client](https://github.com/JamesClonk/vultr)

<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
<!-- providers/dns/vultr/vultr.toml -->
<!-- THIS DOCUMENTATION IS AUTO-GENERATED. PLEASE DO NOT EDIT. -->
