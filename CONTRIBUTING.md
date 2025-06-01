
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
