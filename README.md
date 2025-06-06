A collection of essential React snippets for Zed code editor that boosts your development workflow with smart shortcuts for common React patterns and hooks.

## Features

- 🚀 30+ essential React snippets
- ⚡️ Lightning-fast component scaffolding
- 🎣 All major React hooks support
- 🧩 Common patterns like context providers, prop types, and event handlers
- 📝 JSX and TypeScript friendly

## Installation

1. Open Zed editor
2. Go to \`Extensions\` in the command palette (\`Cmd+K\`)
3. Search for "React Snippets"
4. Click \`Install\`

## Snippet Usage

Type the prefix and press \`Tab\` to expand the snippet. Use \`Tab\` and \`Shift+Tab\` to navigate between placeholders.

## Snippet Reference

### Component Scaffolding

| Prefix   | Description           | Snippet Preview                               |
| -------- | --------------------- | --------------------------------------------- |
| \`rfc\`  | Function component    | \`function Component() { ... }\`              |
| \`rfcp\` | Component with props  | \`function Component({ prop }) { ... }\`      |
| \`rfce\` | Component with export | \`export default function Component() {...}\` |
| \`memo\` | Memoized component    | \`React.memo(Component)\`                     |
| \`frag\` | React Fragment        | \`<></>\`                                     |

### React Hooks

| Prefix          | Description      | Snippet Preview                          |
| --------------- | ---------------- | ---------------------------------------- |
| \`useState\`    | State hook       | \`const [state, setState] = useState()\` |
| \`useEffect\`   | Effect hook      | \`useEffect(() => {...}, [])\`           |
| \`useContext\`  | Context hook     | \`const ctx = useContext(Context)\`      |
| \`useRef\`      | Ref hook         | \`const ref = useRef()\`                 |
| \`useMemo\`     | Memoization hook | \`const value = useMemo(() => ...)\`     |
| \`useCallback\` | Callback hook    | \`const cb = useCallback(() => ...)\`    |

### Event Handlers

| Prefix       | Description           | Snippet Preview                      |
| ------------ | --------------------- | ------------------------------------ |
| \`handler\`  | Generic event handler | \`const handleEvent = (e) => {...}\` |
| \`onClick\`  | Click handler         | \`onClick={handleClick}\`            |
| \`onChange\` | Change handler        | \`onChange={handleChange}\`          |
| \`onSubmit\` | Form submit handler   | \`onSubmit={handleSubmit}\`          |

### Utilities

| Prefix      | Description           | Snippet Preview                     |
| ----------- | --------------------- | ----------------------------------- |
| \`cond\`    | Conditional rendering | \`{condition ? a : b}\`             |
| \`map\`     | Array mapping         | \`{array.map(item => ...)}\`        |
| \`context\` | Context provider      | \`const Context = createContext()\` |
| \`styled\`  | Styled component      | \`const Styled = styled.div\`...    |
| \`ptypes\`  | PropTypes definition  | \`Component.propTypes = {...}\`     |

### Imports

| Prefix   | Description             | Snippet Preview                             |
| -------- | ----------------------- | ------------------------------------------- |
| \`imr\`  | Import React            | \`import React from 'react'\`               |
| \`imrh\` | Import React with hooks | \`import React, { useState } from 'react'\` |
| \`impt\` | Import PropTypes        | \`import PropTypes from 'prop-types'\`      |

## Example Workflow

1. Create a new component file
2. Type \`rfce\` + \`Tab\` to scaffold a component
3. Add state with \`useState\` + \`Tab\`
4. Add effect with \`useEffect\` + \`Tab\`
5. Add click handler with \`onClick\` + \`Tab\`

\`\`\`jsx
function Counter() {
const [count, setCount] = useState(0); // ← useState snippet

useEffect(() => { // ← useEffect snippet
document.title = \`Count: \${count}\`;
}, [count]);

const handleClick = () => { // ← handler snippet
setCount(c => c + 1);
};

return (
<button onClick={handleClick}> // ← onClick snippet
Count: {count}
</button>
);
}

export default Counter;
\`\`\`

## Contributing

Contributions are welcome! To add new snippets:

1. Fork the repository
2. Add your snippets to \`snippets.json\`
3. Submit a pull request

---

**Happy Coding!** 🚀
Boost your React development with these essential Zed snippets.`;
