---
title: The StoreState interface
---
# Intro

This document will cover the interface <SwmToken path="src/types/index.tsx" pos="2:4:4" line-data="export interface StoreState {">`StoreState`</SwmToken>. We will explain:

1. What <SwmToken path="src/types/index.tsx" pos="2:4:4" line-data="export interface StoreState {">`StoreState`</SwmToken> is and its purpose.
2. The variables defined in <SwmToken path="src/types/index.tsx" pos="2:4:4" line-data="export interface StoreState {">`StoreState`</SwmToken>.

# What is <SwmToken path="src/types/index.tsx" pos="2:4:4" line-data="export interface StoreState {">`StoreState`</SwmToken>

<SwmToken path="src/types/index.tsx" pos="2:4:4" line-data="export interface StoreState {">`StoreState`</SwmToken> is an interface defined in <SwmPath>[src/types/index.tsx](src/types/index.tsx)</SwmPath> that represents the shape of the state object used in the store. It is used to type the state managed in the application, ensuring that the state has a consistent structure with specific properties.

<SwmSnippet path="/src/types/index.tsx" line="2">

---

The variable <SwmToken path="src/types/index.tsx" pos="3:1:1" line-data="    languageName: string;">`languageName`</SwmToken> is a string that represents the name of the programming language or language context stored in the state.

```tsx
export interface StoreState {
    languageName: string;
    enthusiasmLevel: number;
}
```

---

</SwmSnippet>

<SwmSnippet path="/src/types/index.tsx" line="2">

---

The variable <SwmToken path="src/types/index.tsx" pos="4:1:1" line-data="    enthusiasmLevel: number;">`enthusiasmLevel`</SwmToken> is a number that indicates the level of enthusiasm or excitement related to the language or context stored in the state.

```tsx
export interface StoreState {
    languageName: string;
    enthusiasmLevel: number;
}
```

---

</SwmSnippet>

&nbsp;

*This is an auto-generated document by Swimm 🌊 and has not yet been verified by a human*

<SwmMeta version="3.0.0" repo-id="Z2l0aHViJTNBJTNBVHlwZVNjcmlwdFhUeXBlU2NyaXB0LVJlYWN0LVN0YXJ0ZXIlM0ElM0FHb3BpbmF0aHJlZGR5NjY=" repo-name="TypeScriptXTypeScript-React-Starter"><sup>Powered by [Swimm](https://app.swimm.io/)</sup></SwmMeta>
