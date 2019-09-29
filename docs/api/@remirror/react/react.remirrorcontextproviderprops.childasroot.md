<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/react](./react.md) &gt; [RemirrorContextProviderProps](./react.remirrorcontextproviderprops.md) &gt; [childAsRoot](./react.remirrorcontextproviderprops.childasroot.md)

## RemirrorContextProviderProps.childAsRoot property

Sets the first child element as a the root (where the prosemirror editor instance will be rendered).

<b>Signature:</b>

```typescript
childAsRoot?: GetRootPropsConfig<string> | boolean;
```

## Remarks

\*\*Example with directly nested components\*\*

When using a remirror provider calling `getRootProps` is mandatory. By setting `childAsRoot` to an object Remirror will inject these props into the first child element.

```tsx
import { ManagedRemirrorProvider, RemirrorManager } from '@remirror/react';

const Editor = () => {
  return (
    <RemirrorManager>
      <ManagedRemirrorProvider childAsRoot={{ refKey: 'ref' }}>
        <div />
      </ManagedRemirrorProvider>
    </RemirrorManager>
  );
}

```
If this is set to an empty object then the outer element must be able to receive a default ref prop which will mount the editor to it. If left undefined then the children components are responsible for calling `getRootProps`<!-- -->.
