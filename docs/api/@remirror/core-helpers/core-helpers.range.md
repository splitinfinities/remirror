<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/core-helpers](./core-helpers.md) &gt; [range](./core-helpers.range.md)

## range variable

Create a range from start to end.

If only start is provided it creates an array of the size provided. if start and end are provided it creates an array who's first position is start and final position is end. i.e. `length = (end - start) + 1`

<b>Signature:</b>

```typescript
range: (start: number, end?: number | undefined) => number[]
```
