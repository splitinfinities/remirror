<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/core](./core.md) &gt; [Extension](./core.extension.md) &gt; [commands](./core.extension.commands.md)

## Extension.commands() method

Register commands for the extension.

These are typically used to create menu's actions and as a direct response to user actions.

<b>Signature:</b>

```typescript
commands?(params: CommandTypeParams<GType>): ExtensionCommandReturn;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  params | <code>CommandTypeParams&lt;GType&gt;</code> | schema params with type included |

<b>Returns:</b>

`ExtensionCommandReturn`

## Remarks

The commands function should return an object with each key being unique within the editor. To ensure that this is the case it is recommended that the keys of the command are namespaced with the name of the extension.

e.g.

```ts
class History extends Extension {
  name = 'history' as const;
  commands() {
    return {
      undoHistory: COMMAND_FN,
      redoHistory: COMMAND_FN,
    }
  }
}

```
The actions available in this case would be `undoHistory` and `redoHistory`<!-- -->. It is unlikely that any other extension would override these commands.

Another benefit of commands is that they are picked up by typescript and can provide code completion for consumers of the extension.

