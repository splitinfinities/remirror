<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/core](./core.md) &gt; [PlainNames](./core.plainnames.md)

## PlainNames type

A utility type for retrieving the name of an extension only when it's a plain extension.

<b>Signature:</b>

```typescript
export declare type PlainNames<GExtension extends AnyExtension> = ProsemirrorTypeOfExtension<GExtension> extends never ? GExtension['name'] : never;
```
