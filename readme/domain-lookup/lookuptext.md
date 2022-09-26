---
description: >-
  This function is able to look up an available EDNS Record.  If the keyword is
  found in the chain, the EDNS will return the record. Otherwise, "undefined"
  will be return while the key.
---

# LookUpText

### Usage

LookUpText(domain: string, type: [TextType](../../broken-reference/)): Promise\<undefined | string>

*   **Parameters**

    * **domain: string**
    * **type:** [**TextType**](../../texttype.md)

    **Returns Promise\<undefined | string>**
