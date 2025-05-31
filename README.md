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

CleanScript is released under the [MIT License](LICENSE).

---

## 📬 Contact

Have questions or suggestions?
Join the discussions on GitHub or open an [issue](https://github.com/your-username/CleanScript/issues).

````

---

### ✅ `CONTRIBUTING.md`

> 📄 Save as: `CONTRIBUTING.md`

```markdown
# 👥 Contributing to CleanScript

Thank you for your interest in contributing to CleanScript! 🎉  
We welcome bug reports, feature requests, improvements, and documentation contributions.

---

## 🧰 Project Setup

1. **Fork this repository** on GitHub.
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/your-username/CleanScript.git
   cd CleanScript
````

3. **Install development dependencies**:

   ```bash
   pip install -e ".[dev,ai]"
   ```

---

## 🚧 Workflow

### 1. Create a Branch

Follow the naming convention: `type/short-description`

Examples:

```bash
git checkout -b feat/ai-docstrings
git checkout -b fix/remove-unused-imports
```

### 2. Make Your Changes

Keep functions small and readable. Add docstrings and type hints where possible.

### 3. Run Tests

Make sure everything passes:

```bash
pytest
```

### 4. Format Code

Ensure the codebase stays consistent:

```bash
black .
isort .
```

### 5. Commit & Push

Follow the conventional commit style:

```bash
git add .
git commit -m "feat(doc): add AI-powered docstring generation"
git push origin feat/doc-improvements
```

Then open a **Pull Request** from your fork.

---

## ✍️ Coding Guidelines

* Follow **PEP 8** style guide.
* Use **type hints** (`def func(x: int) -> str:`).
* Keep functions **< 25 lines** if possible.
* Add or update **tests** for new features.
* Include or update **docstrings**.
* Use **Black** and **isort** for formatting.

---

## 🔖 Commit Message Format

```
type(scope): short description

Optional detailed explanation.
```

### Valid Types:

* `feat` – new feature
* `fix` – bug fix
* `docs` – documentation changes
* `refactor` – code restructuring
* `test` – tests only
* `chore` – build/dependencies/tools

**Examples**:

```
feat(ai): generate AI-based function summaries
fix(format): handle multiline import removal
docs(README): add installation instructions
```

---

## 🆘 Need Help?

* Open an issue with a detailed description.
* Use the GitHub [Discussions](https://github.com/your-username/CleanScript/discussions).
* We’re happy to help you contribute!

````

---

Once added to your project, commit them:

```bash
git add README.md CONTRIBUTING.md
git commit -m "Add detailed README and CONTRIBUTING guide"
git push origin main
````

Let me know if you also want a `LICENSE`, `setup.cfg`, or GitHub Actions workflow template!
