# Using This Template

This repository is a GitHub template. Use it to quickly bootstrap new OpenAI agent projects.

## Method 1: GitHub Web Interface (Recommended)

1. Navigate to the repository: https://github.com/blainemholt/openai-agent-template
2. Click the green **"Use this template"** button
3. Select **"Create a new repository"**
4. Choose a name for your new repository
5. Select public or private visibility
6. Click **"Create repository from template"**
7. Clone your new repository:
   ```bash
   gh repo clone your-username/your-repo-name
   cd your-repo-name
   ```

## Method 2: GitHub CLI

```bash
# Create a new repository from this template
gh repo create your-new-repo-name --template blainemholt/openai-agent-template

# Clone it
gh repo clone your-username/your-new-repo-name
cd your-new-repo-name
```

## Method 3: Manual Setup

```bash
# Clone the template repository
gh repo clone blainemholt/openai-agent-template my-new-project
cd my-new-project

# Remove the old git history
rm -rf .git

# Initialize a new git repository
git init
git branch -m main

# Add and commit files
git add .
git commit -m "Initial commit from template"

# Create a new GitHub repository and push
gh repo create my-new-project --public --source=. --remote=origin --push
```

## After Creating Your Repository

1. **Install dependencies:**
   ```bash
   uv sync
   ```

2. **Set up environment variables:**
   - Copy `.env.example` to `.env` (if it exists) or create a new `.env` file
   - Add your OpenAI API key:
     ```
     OPENAI_API_KEY=your-api-key-here
     ```

3. **Customize the project:**
   - Update `pyproject.toml` with your project name and description
   - Modify `main.py` with your application logic
   - Update `README.md` with your project-specific information
   - Add any additional dependencies you need:
     ```bash
     uv add package-name
     ```

4. **Start developing:**
   ```bash
   # Run your application
   uv run python main.py
   
   # Or start Jupyter notebooks
   uv run jupyter notebook
   ```

## What Gets Copied?

When you use this template, you'll get:
- ✅ All source code files
- ✅ Project configuration (`pyproject.toml`, `uv.lock`)
- ✅ Documentation files
- ✅ Git configuration files (`.gitignore`, etc.)
- ✅ Code quality configuration (`.codacy/`)

You will **NOT** get:
- ❌ Git history (starts fresh)
- ❌ Environment files (`.env` is gitignored)
- ❌ Local development files

## Need Help?

- Check the main [README.md](README.md) for project-specific documentation
- Review the [OpenAI Agents SDK documentation](https://github.com/openai/openai-agents-python)
- Check [uv documentation](https://github.com/astral-sh/uv) for dependency management

