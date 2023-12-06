# ansible-role-wrapper

Wrapper around ansible-playbook to run standalone roles (inside of collections) without playbook.
The wrapper will use ansible-galaxy to search for the role in all available collections path.
After that it will create a temporary playbook for the role and then run it with all given parameters.

## Usage

Symlink the wrapper to a directory in your PATH and use it like **ansible-playbook**.

```bash
ansible-role <role fqcn> [ansible-playbook options]
```
