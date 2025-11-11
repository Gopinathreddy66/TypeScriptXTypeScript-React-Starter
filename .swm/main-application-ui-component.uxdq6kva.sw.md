---
title: Main Application UI Component
---
# introduction

This document explains the main parts of the primary UI component in <SwmPath>[src/App.tsx](src/App.tsx)</SwmPath>. It answers these questions:

1. How is the component structured and what does it render?
2. How are external resources like images and styles integrated?
3. How does the component incorporate child components?

# component structure and rendering

<SwmSnippet path="/src/App.tsx" line="1">

---

The component is a functional React component named <SwmToken path="src/App.tsx" pos="2:4:4" line-data="import &#39;./App.css&#39;;">`App`</SwmToken>. It returns a JSX tree that forms the main UI structure. The root element is a div with class "App". Inside it, there is a header section containing a logo image and a heading. Below the header, there is a paragraph with instructions for editing the file. Finally, it renders a child component called <SwmToken path="src/App.tsx" pos="3:2:2" line-data="import Hello from &#39;./components/Hello&#39;;">`Hello`</SwmToken> with a prop <SwmToken path="src/App.tsx" pos="17:4:4" line-data="      &lt;Hello name=&quot;TypeScript&quot; /&gt;">`name`</SwmToken> set to <SwmToken path="src/App.tsx" pos="17:7:7" line-data="      &lt;Hello name=&quot;TypeScript&quot; /&gt;">`TypeScript`</SwmToken>. This structure defines the visible layout and content of the app's main screen.

```tsx
import * as React from 'react';
import './App.css';
import Hello from './components/Hello';

const logo = require('./logo.svg');

function App() {
  return (
    <div className="App">
      <div className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        <h2>Welcome to React</h2>
      </div>
      <p className="App-intro">
        To get started, edit <code>src/App.tsx</code> and save to reload.
      </p>
      <Hello name="TypeScript" />
    </div>
  );
}
```

---

</SwmSnippet>

# external resources and styling

<SwmSnippet path="/src/App.tsx" line="1">

---

The component imports a CSS file for styling, which applies styles to the classes used in the JSX like "App", <SwmToken path="src/App.tsx" pos="10:7:9" line-data="      &lt;div className=&quot;App-header&quot;&gt;">`App-header`</SwmToken>, and <SwmToken path="src/App.tsx" pos="11:13:15" line-data="        &lt;img src={logo} className=&quot;App-logo&quot; alt=&quot;logo&quot; /&gt;">`App-logo`</SwmToken>. The logo image is imported using a require statement and then used as the source for the img element. This approach bundles the image with the app and allows referencing it in JSX. The alt attribute on the image improves accessibility by providing descriptive text.

```tsx
import * as React from 'react';
import './App.css';
import Hello from './components/Hello';

const logo = require('./logo.svg');

function App() {
  return (
    <div className="App">
      <div className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        <h2>Welcome to React</h2>
      </div>
      <p className="App-intro">
        To get started, edit <code>src/App.tsx</code> and save to reload.
      </p>
      <Hello name="TypeScript" />
    </div>
  );
}
```

---

</SwmSnippet>

# child component usage

<SwmSnippet path="/src/App.tsx" line="1">

---

The <SwmToken path="src/App.tsx" pos="3:2:2" line-data="import Hello from &#39;./components/Hello&#39;;">`Hello`</SwmToken> component is imported from the components folder and used inside the main div. It receives a prop <SwmToken path="src/App.tsx" pos="17:4:4" line-data="      &lt;Hello name=&quot;TypeScript&quot; /&gt;">`name`</SwmToken> with the value <SwmToken path="src/App.tsx" pos="17:7:7" line-data="      &lt;Hello name=&quot;TypeScript&quot; /&gt;">`TypeScript`</SwmToken>. This demonstrates how the main component composes smaller components to build the UI and pass data down via props.

```tsx
import * as React from 'react';
import './App.css';
import Hello from './components/Hello';

const logo = require('./logo.svg');

function App() {
  return (
    <div className="App">
      <div className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        <h2>Welcome to React</h2>
      </div>
      <p className="App-intro">
        To get started, edit <code>src/App.tsx</code> and save to reload.
      </p>
      <Hello name="TypeScript" />
    </div>
  );
}
```

---

</SwmSnippet>

# exporting the component

<SwmSnippet path="/src/App.tsx" line="22">

---

At the end of the file, the <SwmToken path="src/App.tsx" pos="22:4:4" line-data="export default App;">`App`</SwmToken> component is exported as the default export. This allows other parts of the application, like the entry point, to import and render this component as the root of the React app.

```tsx
export default App;
```

---

</SwmSnippet>

&nbsp;

*This is an auto-generated document by Swimm 🌊 and has not yet been verified by a human*

<SwmMeta version="3.0.0" repo-id="Z2l0aHViJTNBJTNBVHlwZVNjcmlwdFhUeXBlU2NyaXB0LVJlYWN0LVN0YXJ0ZXIlM0ElM0FHb3BpbmF0aHJlZGR5NjY=" repo-name="TypeScriptXTypeScript-React-Starter"><sup>Powered by [Swimm](https://app.swimm.io/)</sup></SwmMeta>
