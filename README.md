# Checklist

# 0) Optional but common first step for dev tooling on macOS
`xcode-select --install`

# 1) Homebrew
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

# 2) Add Homebrew to shell
`eval "$(/opt/homebrew/bin/brew shellenv)"`   # Apple Silicon
# or:
`eval "$(/usr/local/bin/brew shellenv)"`      # Intel Mac

`brew --version && which brew`

# 3) uv
`curl -LsSf https://astral.sh/uv/install.sh | sh`
`uv --version`

# 4) Make sure uv-managed Python executables are on PATH if needed
`uv python update-shell`

# 5) Python with uv
`uv python install`
`uv python list`
`uv python find`

# 6) New project
`mkdir my-project && cd my-project`
`uv init`

# 7) Project env
`uv venv`
`source .venv/bin/activate`

# 8) Dependencies
`uv add <packages>`
`uv sync`

# 9) SSH for GitHub
`ls -al ~/.ssh`
`ssh-keygen -t ed25519 -C "your_email@example.com"`
`eval "$(ssh-agent -s)"`
`ssh-add ~/.ssh/id_ed25519`
`pbcopy < ~/.ssh/id_ed25519.pub`

# 10) Then paste key into GitHub > Settings > SSH and GPG keys
`ssh -T git@github.com`

# 11) Building
`brew install git`
`brew install node`
`node -v`
`npm -v`
`npx -v`
