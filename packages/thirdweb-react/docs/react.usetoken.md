<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thirdweb-dev/react](./react.md) &gt; [useToken](./react.usetoken.md)

## useToken() function

Hook for getting an instance of a `Token` contract. This contract supports ERC20 compliant tokens.

<b>Signature:</b>

```typescript
export declare function useToken(contractAddress?: string): Token | undefined;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  contractAddress | string | <i>(Optional)</i> the address of the Token contract, found in your thirdweb dashboard |

<b>Returns:</b>

Token \| undefined

## Example


```javascript
import { useToken } from '@thirdweb-dev/react'

export default function Component() {
  const token = useToken("<YOUR-CONTRACT-ADDRESS>")

  // Now you can use the token contract in the rest of the component

  // For example, this function will get the connected wallets token balance
  async function balance() {
    const balance = await token.balance()
    return balance
  }

  ...
}
```
