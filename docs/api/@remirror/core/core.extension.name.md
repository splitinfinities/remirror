<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/core](./core.md) &gt; [Extension](./core.extension.md) &gt; [name](./core.extension.name.md)

## Extension.name property

The unique name of this extension.

<b>Signature:</b>

```typescript
abstract readonly name: string;
```

## Remarks

Every extension \*\*must\*\* have a name. Ideally the name should have a distinct type to allow for better type inference for end users. By convention the name should be `camelCased` and unique within your editor instance.

```ts
class SimpleExtension extends Extension {
  get name() {
    return 'simple' as const;
  }
}

```

