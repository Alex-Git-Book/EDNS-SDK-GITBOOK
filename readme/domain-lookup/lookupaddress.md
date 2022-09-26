---
description: >-
  This function is able to look up the wallet address for different Tokens of a
  registered EDNS name. "undefined" will be return while the token address does
  not set.
---

# LookupAddress

### Usage

LookupAddress(domain: string, coinName: string): Promise\<undefined | string>

*   **Parameters**

    * **domain: string**
    * **coinName: string (**[**The cryptocurrency name**](../../cryptocurrency-short-name.md)**)**

    **Returns Promise\<undefined | string>**
