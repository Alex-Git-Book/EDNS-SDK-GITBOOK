---
description: >-
  This section is explaining how to use the SDK to set Text Records, wallet
  address for receive different Token, and default domain name.
---

# Domain Set Record

### Examples

To Set up a wallet address "0x14A1A496fABc43bFAfC358005dE336a7B5222b20" for receiving ADA of Domain "ednsdomains2022.meta" .

```
import {WriteAddress, GetEdnsProvider} from "@edns/sdk";

const provider = await GetEdnsProvider()
let walletWithProvider = new ethers.Wallet(privateKey, provider);
 try {
  let result = await WriteAddress("ednsdomains2022.meta","ADA","0x14A1A496fABc43bFAfC358005dE336a7B5222b20",walletWithProvider)
  console.log(result)
}catch (e){
    console.log(e)
}
    
```

To add a GITHUB Link for Domain "ednsdomains2022.meta"

```
import {LookUpText, TextType} from "@edns/sdk";
const provider = await GetEdnsProvider()
let walletWithProvider = new ethers.Wallet(privateKey, provider);
try {
    let result = await WriteText("ednsdomains2022.meta",TextType.GITHUB, "https://github.com/ednsdomains/Edns-sdk",walletWithProvider,)
    console.log(result)
}catch (e){
    console.log(e)
}
```
