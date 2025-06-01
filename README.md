# CleanScript 🧹🤖

[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

CleanScript is an AI-enhanced Python code cleanup and optimization tool that helps developers write cleaner, more maintainable, and documented Python code. Whether you're refactoring legacy scripts or enforcing consistency across a team project, CleanScript does the heavy lifting for you.

---

## ✨ Features

- 🔥 **Remove Unused Imports:** Automatically detect and remove unused imports.
- 🧠 **AI-Powered Docstrings:** Generate docstrings using either templates or AI models.
- 🧼 **Black Integration:** Format your code using the [Black](https://github.com/psf/black) formatter.
- 🧾 **Explain Code with AI:** Get line-by-line explanations of what a function does.
- ✅ **PEP 8 Lint Checks:** Ensure code follows PEP 8 styling guidelines.
- 🔁 **Batch Processing:** Clean an entire project or directory.
- ⚙️ **Custom Config File:** Configure tool behavior with `.cleanscriptrc`.

---

## 📦 Installation

Install using pip:

```bash
# With AI-powered features (requires OpenAI key or similar)
pip install cleanscript[ai]

# Core features only
pip install cleanscript
````

---

## 🚀 Usage

### Basic usage

```bash
cleanscript path/to/file.py
```

### With AI features

```bash
cleanscript path/to/file.py --ai-docstrings --comment-functions
```

### Clean an entire project

```bash
cleanscript path/to/project/ --in-place
```

### Show help

```bash
cleanscript --help
```

---

## ⚙️ Configuration

You can create a `.cleanscriptrc` file in your project root to customize behavior:

```ini
[cleanscript]
ai_docstrings = true
max_line_length = 88
exclude = tests/*,migrations/
```

---

## 🧪 Example

### Before

```python
import os, sys

def process(x):
    return x*2
```

### After

```python
def process(x):
    """Double the input value.

    Args:
        x (int): Input number

    Returns:
        int: Double the input
    """
    return x * 2
```

---

## 🛠 Development

To contribute, please read the [CONTRIBUTING.md](./CONTRIBUTING.md) file for instructions on setting up your development environment.

---

## 🧑‍💻 Contributing

Whether you're fixing bugs, improving documentation, or adding new features—your contributions are welcome!

1. Fork the repository
2. Create a new feature branch (`git checkout -b feat/my-feature`)
3. Commit your changes and push (`git push origin feat/my-feature`)
4. Open a pull request

Please follow the coding conventions and commit guidelines outlined in [CONTRIBUTING.md](./CONTRIBUTING.md).

---

## 📄 License

CleanScript is released under the [MIT License](./LICENSE.txt).

---

## 📬 Contact

Have questions or suggestions?
Join the discussions on GitHub or open an [issue](https://github.com/arunvijo/CleanScript/issues).
