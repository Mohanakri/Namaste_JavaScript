# JavaScript Emmet Cheat Sheet for VS Code

## Basic JavaScript Snippets

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `log` | `console.log()` | Console log |
| `warn` | `console.warn()` | Console warning |
| `error` | `console.error()` | Console error |
| `dir` | `console.dir()` | Console directory |
| `table` | `console.table()` | Console table |

## Functions

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `f` | `function name() {}` | Function declaration |
| `fn` | `function() {}` | Anonymous function |
| `iife` | `(function() {})()` | Immediately Invoked Function Expression |
| `af` | `() => {}` | Arrow function |
| `afn` | `(param) => {}` | Arrow function with parameter |
| `nfn` | `const name = () => {}` | Named arrow function |

## Control Structures

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `if` | `if (condition) {}` | If statement |
| `ife` | `if (condition) {} else {}` | If-else statement |
| `el` | `else {}` | Else block |
| `ei` | `else if (condition) {}` | Else if |
| `sw` | `switch (expr) { case: break; default: }` | Switch statement |
| `case` | `case value: break;` | Case statement |
| `tc` | `try {} catch (e) {}` | Try-catch block |
| `tf` | `try {} finally {}` | Try-finally block |
| `tcf` | `try {} catch (e) {} finally {}` | Try-catch-finally |

## Loops

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `for` | `for (let i = 0; i < array.length; i++) {}` | For loop |
| `fori` | `for (let i = 0; i < length; i++) {}` | For loop with index |
| `forr` | `for (let i = length - 1; i >= 0; i--) {}` | Reverse for loop |
| `forin` | `for (let key in object) {}` | For-in loop |
| `forof` | `for (let item of iterable) {}` | For-of loop |
| `wh` | `while (condition) {}` | While loop |
| `dowhile` | `do {} while (condition)` | Do-while loop |

## Array Methods

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `fe` | `forEach((item) => {})` | ForEach method |
| `map` | `map((item) => {})` | Map method |
| `filter` | `filter((item) => {})` | Filter method |
| `find` | `find((item) => {})` | Find method |
| `reduce` | `reduce((acc, item) => {}, initial)` | Reduce method |
| `some` | `some((item) => {})` | Some method |
| `every` | `every((item) => {})` | Every method |

## Objects & Classes

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `obj` | `const obj = {}` | Object literal |
| `kv` | `key: value,` | Key-value pair |
| `class` | `class Name {}` | Class declaration |
| `ctor` | `constructor() {}` | Constructor |
| `met` | `methodName() {}` | Method |
| `get` | `get propertyName() {}` | Getter |
| `set` | `set propertyName(value) {}` | Setter |

## Promises & Async

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `promise` | `new Promise((resolve, reject) => {})` | Promise constructor |
| `then` | `.then((result) => {})` | Promise then |
| `catch` | `.catch((error) => {})` | Promise catch |
| `async` | `async function name() {}` | Async function |
| `await` | `await promise` | Await expression |
| `af async` | `async () => {}` | Async arrow function |

## Variable Declarations

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `let` | `let variable;` | Let declaration |
| `const` | `const variable = value;` | Const declaration |
| `var` | `var variable;` | Var declaration |
| `dstr` | `const {} = object;` | Destructuring assignment |
| `imp` | `import {} from 'module'` | Import statement |
| `imd` | `import module from 'module'` | Default import |
| `exp` | `export {}` | Export statement |
| `exd` | `export default` | Default export |

## React/JSX Specific

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `rfc` | React Functional Component | Function component template |
| `rcc` | React Class Component | Class component template |
| `useState` | `const [state, setState] = useState()` | useState hook |
| `useEffect` | `useEffect(() => {}, [])` | useEffect hook |
| `ust` | `const [state, setState] = useState()` | useState shorthand |
| `uef` | `useEffect(() => {}, [])` | useEffect shorthand |

## DOM Manipulation

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `qs` | `document.querySelector()` | Query selector |
| `qsa` | `document.querySelectorAll()` | Query selector all |
| `gid` | `document.getElementById()` | Get element by ID |
| `gcn` | `document.getElementsByClassName()` | Get elements by class |
| `gtn` | `document.getElementsByTagName()` | Get elements by tag |
| `ae` | `addEventListener('', () => {})` | Add event listener |
| `re` | `removeEventListener('', handler)` | Remove event listener |

## Utility Snippets

| Abbreviation | Expands To | Description |
|--------------|-----------|-------------|
| `timeout` | `setTimeout(() => {}, delay)` | Set timeout |
| `interval` | `setInterval(() => {}, delay)` | Set interval |
| `json` | `JSON.stringify()` | JSON stringify |
| `parse` | `JSON.parse()` | JSON parse |
| `random` | `Math.random()` | Random number |
| `floor` | `Math.floor()` | Math floor |
| `ceil` | `Math.ceil()` | Math ceiling |

## Tips for Using Emmet in VS Code

1. **Trigger Emmet**: Type the abbreviation and press `Tab` or `Ctrl+Space`
2. **Multiple cursors**: Use `Alt+Click` to create multiple cursors and expand Emmet on all
3. **Custom snippets**: Add custom Emmet snippets in VS Code settings
4. **Enable in other files**: Configure Emmet to work in additional file types via settings

## Settings Configuration

Add to your `settings.json`:
```json
{
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  },
  "emmet.triggerExpansionOnTab": true,
  "emmet.showExpandedAbbreviation": "always"
}
```

Remember: Not all abbreviations work in plain JavaScript files - some are specific to JSX/React or require additional configuration!
