# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Python experimentation project created with PyCharm. The project appears to be in its initial stages with a basic PyCharm template structure.

### Current Status
- **Project Type**: Python experimental/learning project
- **Python Version**: 3.9.6
- **IDE**: PyCharm
- **Virtual Environment**: Yes (`venv/` directory)
- **Version Control**: Git initialized but no commits yet
- **Dependencies**: None installed

## Development Setup

### Virtual Environment
- The project uses a Python 3.9.6 virtual environment located in `venv/`
- Activate the virtual environment before running any Python commands:
  ```bash
  source venv/bin/activate  # On macOS/Linux
  ```

### Dependencies
- Currently no `requirements.txt` file exists
- No packages are installed in the virtual environment
- When adding dependencies:
  ```bash
  pip install <package>
  pip freeze > requirements.txt
  ```

## Project Structure

```
claude-experiments/
├── .git/           # Git repository (initialized but no commits)
├── .idea/          # PyCharm IDE configuration
├── venv/           # Python virtual environment
├── CLAUDE.md       # This file - AI assistant instructions
└── main.py         # Main entry point (PyCharm template)
```

### Code Analysis

**main.py**:
- Contains PyCharm's default template code
- Simple function `print_hi(name)` that prints a greeting
- Entry point that calls `print_hi('PyCharm')`
- Includes helpful PyCharm shortcuts in comments

## Common Commands

### Running the Application
```bash
python main.py
```
Output: `Hi, PyCharm`

### Git Operations
```bash
# First commit (recommended)
git add CLAUDE.md main.py
git commit -m "Initial commit with PyCharm template"

# Add .gitignore before committing more
git add .gitignore
git commit -m "Add .gitignore for Python project"
```

## Missing Components & Recommendations

### Immediate Priorities
1. **Create `.gitignore`** file with:
   ```
   # Virtual Environment
   venv/
   env/
   ENV/
   
   # PyCharm
   .idea/
   
   # Python
   __pycache__/
   *.py[cod]
   *$py.class
   *.so
   .Python
   
   # Distribution / packaging
   build/
   develop-eggs/
   dist/
   downloads/
   eggs/
   .eggs/
   lib/
   lib64/
   parts/
   sdist/
   var/
   wheels/
   *.egg-info/
   .installed.cfg
   *.egg
   
   # Unit test / coverage
   htmlcov/
   .tox/
   .coverage
   .coverage.*
   .cache
   .pytest_cache/
   nosetests.xml
   coverage.xml
   *.cover
   .hypothesis/
   
   # Environments
   .env
   .venv
   ```

2. **Consider project structure** for experiments:
   ```
   claude-experiments/
   ├── experiments/
   │   ├── __init__.py
   │   ├── experiment_01_basics.py
   │   └── experiment_02_advanced.py
   ├── utils/
   │   └── __init__.py
   ├── tests/
   │   └── __init__.py
   └── notebooks/  # If using Jupyter
   ```

### Development Tools to Consider
- **Testing**: pytest
- **Linting**: ruff or flake8
- **Formatting**: black
- **Type Checking**: mypy
- **Documentation**: Add README.md

### Typical Workflow for Experiments
1. Create new experiment files in logical groupings
2. Document findings in docstrings or markdown
3. Consider using Jupyter notebooks for exploratory work
4. Save successful experiments as proper Python modules

## Best Practices for This Repository

1. **Experimentation**: Since this appears to be for experiments, consider:
   - Clear naming for experiment files
   - Good documentation of what each experiment tests
   - Saving both successful and failed experiments with notes

2. **Version Control**: 
   - Commit frequently with descriptive messages
   - Use branches for different experiment types

3. **Dependencies**:
   - Add dependencies as you need them
   - Always update requirements.txt after installing

4. **Code Style**:
   - Follow PEP 8 conventions
   - Use descriptive variable and function names
   - Add docstrings to functions explaining experiments