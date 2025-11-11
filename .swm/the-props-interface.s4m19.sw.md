---
title: The Props interface
---
This document explains the interface Props in <SwmPath>[src/components/Hello.tsx](src/components/Hello.tsx)</SwmPath>. We will cover:

1. What is Props
2. Variables and functions defined in Props

# What is Props

Props in <SwmPath>[src/components/Hello.tsx](src/components/Hello.tsx)</SwmPath> is an interface that defines the shape of the properties passed to the Hello React component. It specifies what data and callbacks the component expects to receive from its parent component, enabling type safety and clear contract for usage.

<SwmSnippet path="/src/components/Hello.tsx" line="4">

---

The variable <SwmToken path="src/components/Hello.tsx" pos="5:1:1" line-data="  name: string;">`name`</SwmToken> is a required string property in Props. It represents the name that will be displayed by the Hello component.

```tsx
export interface Props {
  name: string;
  enthusiasmLevel?: number;
```

---

</SwmSnippet>

<SwmSnippet path="/src/components/Hello.tsx" line="6">

---

The variable <SwmToken path="src/components/Hello.tsx" pos="6:1:1" line-data="  enthusiasmLevel?: number;">`enthusiasmLevel`</SwmToken> is an optional number property in Props. It indicates the level of enthusiasm to be displayed, defaulting to 1 if not provided.

```tsx
  enthusiasmLevel?: number;
  onIncrement?: () => void;
```

---

</SwmSnippet>

<SwmSnippet path="/src/components/Hello.tsx" line="7">

---

The function <SwmToken path="src/components/Hello.tsx" pos="7:1:1" line-data="  onIncrement?: () =&gt; void;">`onIncrement`</SwmToken> is an optional callback function property in Props. It is intended to be called when the user wants to increase the enthusiasm level, typically triggered by a button click.

```tsx
  onIncrement?: () => void;
  onDecrement?: () => void;
```

---

</SwmSnippet>

<SwmSnippet path="/src/components/Hello.tsx" line="8">

---

The function <SwmToken path="src/components/Hello.tsx" pos="8:1:1" line-data="  onDecrement?: () =&gt; void;">`onDecrement`</SwmToken> is an optional callback function property in Props. It is intended to be called when the user wants to decrease the enthusiasm level, typically triggered by a button click.

```tsx
  onDecrement?: () => void;
}
```

---

</SwmSnippet>

&nbsp;

*This is an auto-generated document by Swimm 🌊 and has not yet been verified by a human*

<SwmMeta version="3.0.0" repo-id="Z2l0aHViJTNBJTNBVHlwZVNjcmlwdFhUeXBlU2NyaXB0LVJlYWN0LVN0YXJ0ZXIlM0ElM0FHb3BpbmF0aHJlZGR5NjY=" repo-name="TypeScriptXTypeScript-React-Starter"><sup>Powered by [Swimm](https://app.swimm.io/)</sup></SwmMeta>
