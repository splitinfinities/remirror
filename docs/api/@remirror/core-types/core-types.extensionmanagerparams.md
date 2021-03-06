<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/core-types](./core-types.md) &gt; [ExtensionManagerParams](./core-types.extensionmanagerparams.md)

## ExtensionManagerParams interface

Parameters passed into many of the extension methods.

<b>Signature:</b>

```typescript
export interface ExtensionManagerParams<GSchema extends EditorSchema = EditorSchema> extends ExtensionManagerInitParams<GSchema>, ExtensionTagParams 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [getActions](./core-types.extensionmanagerparams.getactions.md) | <code>ActionGetter</code> | A helper method to provide access to all the editor actions from within an extension. |
|  [getHelpers](./core-types.extensionmanagerparams.gethelpers.md) | <code>HelperGetter</code> | A helper method to provide access to all the helper methods from within an extension. |
|  [schema](./core-types.extensionmanagerparams.schema.md) | <code>GSchema</code> | The Prosemirror schema being used for the current interface |

