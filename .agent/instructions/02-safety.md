# Safety & Environment
- **Dependency Protection**: Never install a new package (`composer require` or `npm install`) unless explicitly asked.
- **Terminal Caution**: Always check if a process is already running on a port (e.g., 8000 for Laravel) before starting a server.
- **Database Safety**: Never run `migrate:fresh` unless confirmed by the user.
