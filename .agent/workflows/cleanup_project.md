---
description: Clean up temporary files and logs in the project workspace
---

This workflow helps you keep the project clean by removing temporary files and identifying unused artifacts.

1.  **Scan for Temporary Files**
    Use `list_dir` to check for common temporary directories or files such as:
    *   `node_modules` (if not needed)
    *   `.log` files
    *   `tmp/` directories
    *   `.DS_Store` files

2.  **Confirm Deletion**
    If any large directories (like `node_modules`) or potentially important logs are found, ask the user for confirmation before deleting.

3.  **Delete Files**
    Use `run_command` with `rm` or `del` commands to remove the identified files.
    
    Example:
    ```powershell
    Remove-Item -Path "path/to/file.log" -Force
    ```

4.  **Verify Cleanup**
    Run `list_dir` again to confirm that the files have been removed.
