Spec-kit setup intallation
1. Install Specify CLI
Choose your preferred installation method:

Option 1: Persistent Installation (Recommended)
Install once and use everywhere:

# From PyPI (recommended)
pip install specifyplus

# Or with uv tools
uv tool install specifyplus

# Upgrade to latest later
pip install -U specifyplus
uv tool upgrade specifyplus
You may uninstall specifyplus:

pip uninstall specifyplus

# or

uv tool uninstall specifyplus
Then use the tool directly:

specifyplus init <PROJECT_NAME>
# or
sp init <PROJECT_NAME>
specifyplus check
# or
sp check
To upgrade specify run:

uv tool install specify-cli --force --from git+https://github.com/github/spec-kit.git
Option 2: One-time Usage
Run directly without installing:

uvx specifyplus --help
uvx specifyplus init <PROJECT_NAME>
# or
uvx sp init <PROJECT_NAME>
Benefits of persistent installation:

Tool stays installed and available in PATH
No need to create shell aliases
Better tool management with uv tool list, uv tool upgrade, uv tool uninstall
Cleaner shell configuration
2. Establish project principles
Use the /sp.constitution command to create your project's governing principles and development guidelines that will guide all subsequent development.

/sp.constitution Create principles focused on code quality, testing standards, user experience consistency, and performance requirements
3. Create the spec
Use the /sp.specify command to describe what you want to build. Focus on the what and why, not the tech stack.

/sp.specify Build an application that can help me organize my photos in separate photo albums. Albums are grouped by date and can be re-organized by dragging and dropping on the main page. Albums are never in other nested albums. Within each album, photos are previewed in a tile-like interface.
4. Create a technical implementation plan
Use the /sp.plan command to provide your tech stack and architecture choices.

/sp.plan The application uses Vite with minimal number of libraries. Use vanilla HTML, CSS, and JavaScript as much as possible. Images are not uploaded anywhere and metadata is stored in a local SQLite database.
5. Break down into tasks
Use /sp.tasks to create an actionable task list from your implementation plan.

/sp.tasks
6. Execute implementation
Use /sp.implement to execute all tasks and build your feature according to the plan.

/sp.implement
