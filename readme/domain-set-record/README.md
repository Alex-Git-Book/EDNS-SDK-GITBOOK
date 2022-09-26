---
description: >-
  This section explains how to use the SDK to set text records and wallet
  addresses for receiving different tokens.
---

# Domain Set Record

[WriteAddress](writeaddress.md)

[WriteText](writetext.md)

### Examples

To set up a wallet address "0x14A1A496fABc43bFAfC358005dE336a7B5222b20" for receiving ETH for domain name "ednsdomains2022.meta" .

```
import {WriteAddress, GetEdnsProvider} from "@edns/sdk";
const privateKey = 'xxx...'
const provider = await GetEdnsProvider()
let walletWithProvider = new ethers.Wallet(privateKey, provider);
 try {
  let result = await WriteAddress("ednsdomains2022.meta","ETH","0x14A1A496fABc43bFAfC358005dE336a7B5222b20",walletWithProvider)
  console.log(result)
}catch (e){
    console.log(e)
}
    
```

To add a GITHUB Link for Domain "ednsdomains2022.meta"

```
import {WriteText, TextType,GetEdnsProvider} from "@edns/sdk";
const privateKey = 'xxx...'
const provider = await GetEdnsProvider()
let walletWithProvider = new ethers.Wallet(privateKey, provider);
try {
    let result = await WriteText("ednsdomains2022.meta",TextType.GITHUB, "https://github.com/ednsdomains/Edns-sdk",walletWithProvider,)
    console.log(result)
}catch (e){
    console.log(e)
}
```
