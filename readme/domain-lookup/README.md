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

To look up a wallet address for receiving ETH of Domain "apexlegend.404" .

```
import {LookupAddress} from "@edns/sdk";

const domain = "apexlegend.404";
const cryptocurrencies = "ETH";
const address = await LookupAddress(domain,cryptocurrencies);

//Return 0x5d6fdbffd6dc6e8a0b69a52dbf010efd905fb7ad
```

To look up a DESCRIPTION of Domain "apexlegend.404"

```
import {LookUpText, TextType} from "@edns/sdk";
const domain = "apexlegend.404"
const record_DESCRIPTION = await LookUpText(domain,TextType.DESCRIPTION)

//Return Apex Legend
```
