---
description: >-
  This function looks up the wallet address for different Tokens of a registered
  EDNS domain name. "undefined" will be returned if the token address has not
  been set.
---

# LookupAddress

### Usage

LookupAddress(domain: string, coinName: string): Promise\<undefined | string>

*   **Parameters**

    * **domain: string**
    * **coinName: string (**[**The cryptocurrency name**](../../cryptocurrency-short-name.md)**)**

    **Returns Promise\<undefined | string>**
