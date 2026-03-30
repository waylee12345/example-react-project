# How to Use GitHub Copilot to Help Code with React?

## Super Autocomplete
You can write comments in the code that explain what the next lines do and let Copilot write (autocomplete) the code.

### Example 1
In line 19 of [App.jsx](my-vite-app/src/App.jsx), you could insert:

```jsx
 {/* add a new div and h1 tag that says "welcome to Vite + React" */}
```

And then Copilot would suggest the next two lines:

```jsx
{/* add a new div and h1 tag that says "welcome to Vite + React" */}
<div className="welcome">
<h1>Get started</h1>
```

### Example 2
In line 10 of [App.jsx](my-vite-app/src/App.jsx), you could insert:

```jsx
// define new state variable to track the number of ticks
```

And then Copilot would suggest the next line:

```jsx
// define new state variable to track the number of ticks
const [ticks, setTicks] = useState(0)
```

## Ask Questions
You can also ask Copilot to answer questions about the code. 

### Example 3
Select a piece of the code, right click, and choose `Explain`. For example,
if you select `src={heroImg}` in line 14 in [App.jsx](my-vite-app/src/App.jsx), you 
get an explanation like:

```text
This line of JSX code sets the src attribute of an HTML <img> element to the value stored in the JavaScript variable heroImg. In React, JSX allows embedding JavaScript expressions within curly braces {} to dynamically assign values to attributes, making the image source reactive to changes in the component's state or props.

(...)
```

## Review Code
Copilot can also help review code to check if something can be fixed.

### Example 4
If you insert an HTML comment within the output of the App component in [App.jsx](my-vite-app/src/App.jsx), this would break the page. For example, in line 24 right before the button, you could add:

```jsx
<!-- indicate the count number and advance it if the button is clicked -->
```

Then, you could select that comment, right click, and select `Review`. Copilot will then bring up the issue that HTML comments are not allowed where that comment was added and provide a suggestion to change the comment format to a JSX compatible comment.


## Modify Code
Copilot can also help modify code, making edits directly onto a file. 

### Example 5
Select the button on lines 27-32 of [App.jsx](my-vite-app/src/App.jsx), right click, select `Modify` and enter `turn the button into an independent and reusable react component`. Then, Copilot will generate a component for the button and insert it in its prior location.