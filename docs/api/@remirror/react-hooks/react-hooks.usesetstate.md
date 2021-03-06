<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@remirror/react-hooks](./react-hooks.md) &gt; [useSetState](./react-hooks.usesetstate.md)

## useSetState variable

A replication of the setState from class Components.

<b>Signature:</b>

```typescript
useSetState: <GState extends object>(initialState?: GState | (() => GState)) => readonly [GState, DispatchWithCallback<PartialSetStateAction<GState>>, (callback?: (() => void) | undefined) => void]
```

## Remarks

It also åaccepts partial updates to the state object and a callback which runs when the state has updated.

It also returns a 3rd argument which resets the state to the original initialState.

```ts
const [state, setState, resetState] = useSetState({a: 'initial', b: 'initial'});

setState({a: 'A'});
log(state); // => { a: 'A', b: 'initial' }

setState(prevState => ({b: 'B'}));
log(state); // => { a: 'A', b: 'B' }

resetState();
log(state); // => { a: 'initial', b: 'initial' }

```

