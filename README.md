# tldr: Your new CLI tool for Python
 
[![Version](https://img.shields.io/pypi/v/tldrcli?color=red&label=version)](https://pypi.org/project/tldrcli/)
[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Language](https://img.shields.io/badge/language-Python-brightgreen.svg)](#)
![Downloads](https://static.pepy.tech/badge/tldrcli)

---

## What is tldr?

**tldr** is a lightweight command-line tool that helps you quickly understand Python error messages and suggests quick fixes so you can debug faster and code smarter. It is built to accommodate all experience levels, helping beginners gain a clearer understanding of Python errors while enabling more advanced users to save time during the debugging process. It natively handles errors and provides solutions (and edits files if needed) for most basic cases, though it has AI support if needed. All local, no API keys needed!

---

## Features

- Looks through your Python tracebacks and explains errors in plain English
- Simple CLI interface: run `tldr <filename>.py` to get instant feedback
- Experimental `--autofix` option to automatically fix errors  
- Tons of internal flags for ease of use
- Native error handling, but has AI-powered fallback  
- Minimal dependencies for easy installation and usage

---

## Installation

Install **tldr** directly in your terminal:

```
pip install tldrcli
```
That's it! **tldr** is ready to use!

## Using tldr

Using **tldr** is as simple as running your Python file, but without typing `python` first. Instead of:
```
python <filename>.py
```
You just type:
```
tldr <filename>.py
```

If your script runs without errors, **tldr** will quietly exit (no unnecessary noise). However, if something does go wrong, **tldr** will instantly catch the error, explain it in plain English,
and even suggest possible fixes right away. The table below shows some of the things tldr can do:

```bash
tldr <filename>.py               # Run code and explain error
tldr --help | -h                 # Show quick docs 
tldr --demo | -d                 # Creates demo file to you to test tldr
tldr --version | -v              # Show current version
tldr --reset | -r                # Reset and clear all data 
tldr <filename>.py --autofix     # Experimental auto-fix mode
tldr --ol | -o                   # Setup instructions for complex --autofix
tldr --oc | -c                   # Verify setup
tldr --stats | -s                # View usage statistics and error history
```
After installing tldr, run ```tldr --help``` to view all available commands. For a hands-on example, run ```tldr --demo``` to generate a sample file you can experiment with. Like this, **tldr** is already a great tool for Python beginners to learn and understand. However, there are always some errors that it cannot predict. To ensure that **tldr** can help you regardless of the situation, set up the local AI model by following the steps in the flag ```tldr --ol```. Once that is done, running ```tldr --oc``` will verify if the setup was done correctly. Below are the same steps you will find in your terminal if you choose to install it later:

- In your terminal, run ```pip install ollama```
- Visit https://ollama.com/ and download the installer
- Run the installer and follow the setup instructions
- Once installed, open a terminal and run ```ollama run llama3:8b```

---

## Contributing
Contributions, issues, and feature requests are welcome! Feel free to open issues to report bugs, request features, submit pull requests to improve the codebase, or more!

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
Devanshu Pandya, pandyadevh@gmail.com
