<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/core-utils](./core-utils.md) &gt; [findChildren](./core-utils.findchildren.md)

## findChildren variable

Iterates over descendants of a given `node`<!-- -->, returning child nodes predicate returns truthy for.

<b>Signature:</b>

```typescript
findChildren: ({ node, predicate, descend }: FindChildrenParams) => NodeWithPosition[]
```

## Remarks

It doesn't descend into a node when descend argument is `false` (defaults to `true`<!-- -->).

```ts
const textNodes = findChildren(node, child => child.isText, false);

```

