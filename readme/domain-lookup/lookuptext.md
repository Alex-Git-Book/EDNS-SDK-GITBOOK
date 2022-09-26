---
description: >-
  This function looks up an available EDNS Record.  If the keyword is found in
  the chain, the relevant record will be returned. Otherwise, "undefined" will
  be returned.
---

# LookUpText

### Usage

LookUpText(domain: string, type: [TextType](../../broken-reference/)): Promise\<undefined | string>

*   **Parameters**

    * **domain: string**
    * **type:** [**TextType**](../../texttype.md)

    **Returns Promise\<undefined | string>**
