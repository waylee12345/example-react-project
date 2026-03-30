# How to Use GitHub Copilot to Help Code with React?

## Super Autocomplete
You can write comments in the code that explain what the next lines do and let Copilot write (autocomplete) the code.

For example, in line 19 of [App.jsx](my-vite-app/src/App.jsx), you could insert:

```jsx
 {/* add a new div and h1 tag that says "welcome to Vite + React" */}
```

And then Copilot would add the next two lines:

```jsx
{/* add a new div and h1 tag that says "welcome to Vite + React" */}
<div className="welcome">
<h1>Get started</h1>
```