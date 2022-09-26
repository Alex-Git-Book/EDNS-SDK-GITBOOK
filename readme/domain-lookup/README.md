# Domain Lookup

This section explains how the SDK looks up Text Records and Wallet Addresses by inputting the relevant EDNS domain.&#x20;

### Available functions

[LookUpText](lookuptext.md)

[LookUpAddress](lookupaddress.md)

### Examples

To look up the ETH wallet address for domain name "apexlegend.404" .

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
