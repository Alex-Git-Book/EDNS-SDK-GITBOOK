---
description: >-
  This section is explaining how to use the SDK to lookup Text Records, Wallet
  Address by using the EDNS Domain. Also including lookup default domain name by
  using wallet address
---

# Domain Lookup

### Available functions

[LookUpText](lookuptext.md)

[LookUpAddress](lookupaddress.md)

[LookupDomainFromAddress](../register-domain/lookupdomainfromaddress.md)

### Examples

A. To lookup a EDNS record

```
import {LookupAddress, LookUpText, TextType} from "@edns/sdk";

const domain = "apexlegend.404";

const cryptocurrencies = "ETH";
const address = await LookupAddress(domain,cryptocurrencies);
const description = await LookUpText(domain,TextType.DESCRIPTION);
```

B. To lookup a domain with a wallet address

```
import {LookupDomainFromAddress} from "@edns/sdk";
const address = "0xCD58F85e6Ec23733143599Fe0f982fC1d3f6C12c"
const domain = await LookupDomainFromAddress(address);
```
