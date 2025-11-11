# OpenAI Agent Template

A template repository for building OpenAI agent applications with Python, Jupyter notebooks, and modern tooling.

## Features

- 🐍 Python 3.12+ with `uv` for fast dependency management
- 🤖 OpenAI Agents SDK integration
- 📓 Jupyter Notebook support
- 🔍 Codacy code quality checks
- 📦 Modern Python project structure with `pyproject.toml`

## Quick Start

### Using this Template

1. Click the **"Use this template"** button on GitHub
2. Create a new repository from the template
3. Clone your new repository:
   ```bash
   gh repo clone your-username/your-repo-name
   cd your-repo-name
   ```
4. Install dependencies:
   ```bash
   uv sync
   ```
5. Set up your environment variables:
   ```bash
   cp .env.example .env  # If you have one, or create .env
   # Add your OpenAI API key: OPENAI_API_KEY=your-key-here
   ```
6. Start coding!

### Local Development

```bash
# Install dependencies
uv sync

# Run the main script
uv run python main.py

# Start Jupyter Notebook
uv run jupyter notebook

# Or start JupyterLab
uv run jupyter lab
```

## Project Structure

```
.
├── main.py              # Main application entry point
├── pyproject.toml       # Project dependencies and metadata
├── uv.lock              # Locked dependency versions
├── README.md            # This file
└── .env                 # Environment variables (not committed)
```

## Dependencies

- `openai-agents` - OpenAI Agents SDK
- `jupyter` - Jupyter notebook support
- `notebook` - Jupyter notebook server

## Environment Variables

Create a `.env` file in the root directory with:

```
OPENAI_API_KEY=your-api-key-here
```

## Customization

After creating a repository from this template:

1. Update `pyproject.toml` with your project name and description
2. Modify `main.py` with your application logic
3. Add your own dependencies as needed:
   ```bash
   uv add package-name
   ```
4. Update this README with your project-specific information

## Code Quality

This template includes Codacy for code quality checks. The configuration is in `.codacy/codacy.yaml`.

## License

[Add your license here]

## Contributing

[Add contribution guidelines if applicable]

