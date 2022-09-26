---
description: >-
  This function looks up the default EDNS domain by inputting its relevant
  wallet address.
---

# Reverse Domain

### Available Function

[SetReverseDomain](setreversedomain.md)

[LookupDomainFromAddress](lookupdomainfromaddress.md)

### Example

To set a reverse domain "ednsdomains2022.meta" for address.

```
import {GetEdnsProvider, SetReverseDomain} from "@edns/sdk";
const privateKey = 'xxx...'
const provider = await GetEdnsProvider()
let walletWithProvider = new ethers.Wallet(privateKey, provider);
try {
    let result = await SetReverseDomain("ednsdomains2022.meta",walletWithProvider)
    console.log(result)
}catch (e){
    console.log(e)
}
```

To look up the EDNSdomain of "0xCD58F85e6Ec23733143599Fe0f982fC1d3f6C12c".

```
import {LookupDomainFromAddress} from "@edns/sdk";
let address = "0xCD58F85e6Ec23733143599Fe0f982fC1d3f6C12c"
console.log(await LookupDomainFromAddress(address));

//return ednsdomains2022.meta
```
