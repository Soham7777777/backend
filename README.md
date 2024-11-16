## Flaskinit : Startup template to create distributable flask webapp
---

### Features:
- Custom Unix compliant CLI script, run `appcli` after installing the project, see `appcli --help` page.
- Fully installable and distributable to a package index like PyPi, so no need to do `git clone ...` the webapp just do `pip install ...`.
- Constrained with all best practices e.g. configuration as `.toml` files.

### How to use this template:
- Clone this, install requirements, make it yours by editing `pyproject.toml` and customize the app and its CLI.
- You can do `pip install -e .` to test the custom script.
- Write tests, they are shiped with distribution.
- When the application is ready to deply just build it: `python3 -m build`, upload the distribution files to PyPi. `pip install <package-name>` to server and provide `.toml` configuration files, run `<yourcli> --help` to check configuration path.
- Optionally, provide `.flaskenv` file(can copy-paste from here) to CWD to change behaviour.