# Checklist

- `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- `brew --version`
- `curl -LsSf https://astral.sh/uv/install.sh | sh`
- `uv --version` 
- `uv python install | uv python list | uv python find`
- `mkdir my-project && cd my-project`
- `uv venv <my-venv-name-or-none>`
- `source <my-venv-name-or-.venv>/bin/activate`
- `uv add <packages>`
- `uv sync`
- `ssh-keygen -t ed25519 -C "your_email@example.com"`
- `eval "$(ssh-agent -s)"`
- `ssh-add ~/.ssh/id_ed25519`
- `pbcopy < ~/.ssh/id_ed25519.pub`
- `ssh -T git@github.com`
