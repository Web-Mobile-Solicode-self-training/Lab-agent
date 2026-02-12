# State Management
- **Persistence**: Maintain a `current_step.txt` file in the root if the task requires multiple sessions.
- **Context Recovery**: Read this file first upon restart to know exactly where the work stopped.
