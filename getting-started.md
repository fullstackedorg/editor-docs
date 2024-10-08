# Getting Started

Once installed, you can now create projects within FullStacked.
Follow along to create a `Hello World` sample project.

## Creating a new project

Start by creating a new project by clicking on the plus `+` tile.

![Projects View](/images/sample-project/projects.png)

Make sure to add a title to your project and if you'd like, select a location where to store your project directory.

![New Project View](/images/sample-project/new-project.png)

## Editing the JavaScript entrypoint

This is file FullStacked will build and bundle expecting to be run in the web view later on.
Let's start by creating a little something.

```js
// index.js
const container = document.createElement("div");
document.body.append(container);
container.innerText = await rpc().greeting("World");
```

![index.js](/images/sample-project/index-js.png)

## Editing the Project entrypoint

We're almost ready to launch your project. 
Like any web-like project, everything starts with an `index.html`.
Let's create it and then add your JS script.

```html
<!-- index.html -->
<script type="module" src="index.js"></script>
```

![index.html](/images/sample-project/index-html.png)

## Running your project

Now we're ready. Run your project.

![Run](/images/sample-project/run.png)

![Sample Project](/images/sample-project/sample-project.png)

## Adding some styling

To spice things up, let's add a bit of styling.
Create a `css` file and add any kind of style attributes you'd like.

```css
/* index.css */
html, body {
    font-family: sans-serif;
    background-color: midnightblue;
    color: whitesmoke;
    height: 100%;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content:center;
}
```

![index.css](/images/sample-project/index-css.png)

Then make sure to add it to your `index.html`.

```html
<!-- index.html -->
<link rel="stylesheet" href="index.css" />
<script type="module" src="index.js"></script>
```

![index.html with css](/images/sample-project/index-html-with-css.png)

Rerun your project and voilà!

![Sample Project with css](/images/sample-project/sample-project-with-css.png)
