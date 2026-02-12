---
description: Scaffold a new component with basic structure
---

This workflow helps you quickly set up a new component directory with standard files.

1.  **Ask for Component Name**
    Ask the user: "What is the name of the new component?" and wait for their response.

2.  **Create Component Directory**
    Create a new directory for the component in `c:\websites\Lab-agent\project\` using the provided name.
    
    ```bash
    mkdir c:\websites\Lab-agent\project\[ComponentName]
    ```

3.  **Create Base Files**
    Create the following files within the new component directory:

    *   `index.html`: A basic HTML5 template.
    *   `style.css`: An empty CSS file.
    *   `script.js`: An empty JavaScript file.

    Use `write_to_file` to create these files.

    **index.html template:**
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>[ComponentName]</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <div class="container">
            <h1>[ComponentName]</h1>
        </div>
        <script src="script.js"></script>
    </body>
    </html>
    ```
