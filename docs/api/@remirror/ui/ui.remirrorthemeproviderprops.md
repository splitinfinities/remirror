<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/ui](./ui.md) &gt; [RemirrorThemeProviderProps](./ui.remirrorthemeproviderprops.md)

## RemirrorThemeProviderProps interface

<b>Signature:</b>

```typescript
export interface RemirrorThemeProviderProps 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [children](./ui.remirrorthemeproviderprops.children.md) | <code>ReactElement</code> | All providers must have ONE child element. |
|  [disableMerge](./ui.remirrorthemeproviderprops.disablemerge.md) | <code>DisableMerge[]</code> | By default the theme provided by this component will be merged with a parent RemirrorTheme or, in the case of the root theme, with the <code>baseTheme</code> and outer emotion theme.<!-- -->Set this to true to disable merging and hence to cause the theme provided to be the only theme used for all nested components.<!-- -->Set this to an array of values to disable against<!-- -->- parent - disable merging with the ancestors - base - disable root providers merging with the base theme - emotion - disable merging with any outer emotion themes |
|  [initialColorMode](./ui.remirrorthemeproviderprops.initialcolormode.md) | <code>string</code> | The initial color mode that will be used when the app is first loaded.<!-- -->It is up to you to decide how this can be persisted between sessions. For example if a user switches to dark mode then reloads the page their settings would be lost.<!-- -->To prevent this you could: - store the mode in local storage and set the color mode to reflect this - With SSR this will always lead to a flash of unstyled content since the color mode can only be retrieved once the DOM loads - store the mode in a cookie session and render the app with this color mode set from the server session. |
|  [theme](./ui.remirrorthemeproviderprops.theme.md) | <code>Partial&lt;RemirrorTheme&gt; &#124; ((currentTheme: RemirrorTheme) =&gt; RemirrorTheme)</code> | The theme being passed into the context.<!-- -->This can either be an object or a function that takes the currentTheme or a default theme when this is the root as the only parameter. It must return a valid <code>RemirrorTheme</code> |
|  [withoutEmotion](./ui.remirrorthemeproviderprops.withoutemotion.md) | <code>boolean</code> | Removes the emotion injected styles from the component. |

