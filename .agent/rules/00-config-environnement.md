---
trigger: always_on
---

# Coding Rules & Constraints

- **Consistency First:** Always match the existing indentation (Tabs vs Spaces) and naming conventions (camelCase vs snake_case) of the file you are editing.
- **No Ghost Dependencies:** Do not import libraries that are not listed in `package.json`. If a new library is needed, ask the user to install it first.
- **Clean Diffs:** Do not refactor entire files if the task only requires changing one function. Keep the "diff" as small as possible.
- **Modern Standards:** Default to ES6+ (Optional chaining, arrow functions) unless the `package.json` indicates an older environment.
- **Error Handling:** Every new function must include basic error handling (try/catch) or null checks.