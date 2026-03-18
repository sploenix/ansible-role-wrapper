# ansible-role-wrapper

Wrapper around `ansible-playbook` to run standalone roles (inside collections) without a playbook.
The wrapper uses `ansible-galaxy` to search for the role in all available collection paths.
After that it creates a temporary playbook for the role and runs it with all given parameters.

## Usage

Install the project, then run it like `ansible-playbook`:

```bash
ansible-role <role fqcn> [ansible-playbook options]
```

## Installation

### Pip

```bash
pip install .
```

### uv

```bash
uv sync
```

## Requirements

- Python 3.9+
- `ansible-playbook` and `ansible-galaxy` available in your `PATH`
