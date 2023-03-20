# mouse-follower-button

## Table of contents

1. [Built with](#built-with)
2. [What I learned](#what-i-learned)
3. [Continued development](#continued-development)
4. [Author](#author)

### Built with

- CSS Paint API
- CSS Properties and Values API
- CSS Custom Variables
- CSS Animation

### What I learned

- **CSS Paint API** allows us to create custom paints using JS and apply them to the CSS properties such as backdround, border etc. It uses a worklet, which is a bit like a worker, that is, a thread running parallel to the main browser thread. Essentially, this means that the worklet won't block the browser from doing other processes;
- <ins>To create a paint worklet</ins>:
    1. Create a separate `workletModule.js` file and define a class with `paint(context, geometry, properties) {}` function inside it;
    2. Register the paint worklet with `registerPaint(workletUniqueName, className)` function to be able to use it;
    3. Add a paint worklet as a module using the `addModule()` method on the **paintWorklet** object of CSS, which will look something like **CSS.paintWorklet.addModule("workletModule.js")**;
    4. Finally, we can use the registered and added to the web page paint worklet in CSS wherever we may expect an image.
- **CSS Custom Properties** are known as CSS Variables allow us to store a value once and use that value with CSS `var()` function in several CSS declarations;
-  **CSS Properties and Values API** allow us to register custom CSS properties with JS `registerProperty()` method and define their initial value, the syntax they are based on, and whether the value inherits down the HTML DOM tree.

### Continued development

- Research and learn other CSS Houdini APIs provided by Houdini: [Is Houdini Ready Yet](https://ishoudinireadyyet.com/)

### Links

- Live Site URL: [Mouse Follower Button](https://mouse-follower-button-karlakz.netlify.app/)

### Author

- Linkedin - [Karlygash Yakiyayeva](https://www.linkedin.com/in/karlygash-yakiyayeva-452baa186/)