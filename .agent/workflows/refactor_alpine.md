---
description: Refactor a component from vanilla JS to Alpine.js
---

This workflow guides you through the process of refactoring a component to use Alpine.js, ensuring consistency with the project's architecture.

1.  **Identify Component**
    Ask the user: "Which component would you like to refactor?" and wait for their response. verify the component exists.

2.  **Analyze Logic**
    Read the `script.js` (or relevant JS file) of the component.
    Identify the state variables and functions that need to be migrated to Alpine.js data and methods.

3.  **Check Base Component**
    Check `c:\websites\Lab-agent\project\baseComponent.js`.
    Ensure any shared logic (like initialization or common utilities) is present or can be reused.

4.  **Refactor HTML**
    Modify the `index.html` file:
    *   Add `x-data` to the root element of the component.
    *   Bind state variables using `x-text`, `x-model`, etc.
    *   Bind event listeners using `x-on:click`, `x-on:submit`, etc.
    *   Ensure `x-cloak` is used to prevent flash of unstyled content if necessary.

    Example structure:
    ```html
    <div x-data="myComponent()">
        <span x-text="message"></span>
        <button @click="updateMessage()">Update</button>
    </div>
    ```

5.  **Remove Old JS**
    Once the Alpine.js implementation is verified, delete the `script.js` file or remove the old logic if it was inline.

6.  **Verify Functionality**
    Open the component in a browser (if possible) or review the code to ensure all original functionality is preserved.
