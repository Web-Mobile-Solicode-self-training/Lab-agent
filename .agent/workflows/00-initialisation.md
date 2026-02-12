# Workflow: Agent Initialization
**Description**: The mandatory standard for starting any task or session.

## Phase 1: Context Mastery
1. **Persona Check**: Read `.agent/rules/01-identite-persona.md` to align role.
2. **Environment Audit**: 
   - Check for `package.json`, `composer.json`, and `.env`.
   - Read `routes/web.php` and `database/migrations` for Laravel projects.
3. **Goal Recognition**: Read the `README.md` or latest task log in `capacity/` to understand the current objective.

## Phase 2: Alignment
- State the detected **Tech Stack**.
- State the **Current Goal** as understood from context.
- Wait for user confirmation before proceeding to **Phase 2: Strategic Planning**.

## Phase 3: Strategic Planning
- Create/Update a `task.md` or `todo.md` in the `capacity/` folder.
- List all files to be modified or created.
- Request user approval.
