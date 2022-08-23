<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thirdweb-dev/react](./react.md) &gt; [MintNFTReturnType](./react.mintnftreturntype.md)

## MintNFTReturnType type

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.
> 

The return type of the [useMintNFT()](./react.usemintnft.md) hook.

<b>Signature:</b>

```typescript
export declare type MintNFTReturnType<TContract> = TContract extends Erc721 ? Awaited<ReturnType<Erc721Mintable["to"]>> : TContract extends Erc1155 ? Awaited<ReturnType<Erc1155Mintable["to"]>> : never;
```