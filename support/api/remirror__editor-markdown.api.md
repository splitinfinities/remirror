## API Report File for "@remirror/editor-markdown"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { FC } from 'react';
import { RemirrorContentType } from '@remirror/core';
import { RemirrorProps } from '@remirror/react';
import { RemirrorProviderProps } from '@remirror/react';

// @public (undocumented)
export type EditorDisplay = 'markdown' | 'wysiwyg';

// @public
export type InternalEditorProps = Omit<RemirrorProviderProps, 'childAsRoot' | 'children'>;

// Warning: (ae-forgotten-export) The symbol "MarkdownEditorProps" needs to be exported by the entry point index.d.ts
// 
// @public (undocumented)
export const MarkdownEditor: FC<MarkdownEditorProps_2>;

// @public (undocumented)
export interface MarkdownEditorProps extends Partial<Pick<RemirrorProps, 'initialContent' | 'attributes' | 'editable' | 'autoFocus' | 'onChange' | 'onFocus' | 'onBlur' | 'onFirstRender' | 'onDispatchTransaction' | 'label' | 'editorStyles' | 'forceEnvironment'>> {
}


// (No @packageDocumentation comment for this package)

```
