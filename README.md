# Weather MCP Project

This project demonstrates the use of Model Context Protocol (MCP) with Python 3.11+.

## Setup

This project requires Python 3.10 or higher. The setup uses pyenv for Python version management.

### Prerequisites

1. **Install pyenv** (if not already installed):
   ```bash
   brew install pyenv
   ```

2. **Add pyenv to your shell configuration**:
   ```bash
   echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
   echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
   echo 'eval "$(pyenv init -)"' >> ~/.zshrc
   source ~/.zshrc
   ```

3. **Install Python 3.11**:
   ```bash
   pyenv install 3.11.9
   ```

### Project Setup

1. **Set the local Python version**:
   ```bash
   cd weather
   pyenv local 3.11.9
   ```

2. **Create and activate virtual environment**:
   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -e .
   ```

## Usage

Once set up, you can use the MCP CLI:

```bash
# Show MCP version
mcp version

# Show help
mcp --help

# Run MCP server with inspector
mcp dev

# Run MCP server
mcp run

# Install MCP server in Claude desktop app
mcp install
```

## Dependencies

- Python >= 3.10
- mcp[cli] - Model Context Protocol CLI tools

## Troubleshooting

If you encounter Python version issues, ensure you're using Python 3.10 or higher:

```bash
python --version
```

The project is configured to use Python 3.11.9 via pyenv.
