# AGENTS.md

## Build/Lint/Test Commands

This repository contains Python scripts for Fermi-LAT data analysis using Fermipy and related tools. No explicit build system detected.

### Testing
There are no explicit test files or framework identified. For running individual scripts:
- `python tracing_TS.py` - Main analysis pipeline
- `python fermi_utils.py` - Utility functions  
- `python Basic_calc_num.py` - Numerical computation utilities

### Linting
No linter configuration detected. For linting, use standard Python tools:
- `flake8 .` - Python style checking
- `pylint *.py` - Python static analysis

### Code Style Guidelines

#### Python Conventions
- Follow PEP 8 style guide for Python code
- Use 4-space indentation
- Maximum line length of 79 characters for code, 79 for docstrings
- Use meaningful variable names (avoid single letter variables except for iterators)
- Use underscores for function names and module names
- Use CamelCase for class names

#### Imports
- Standard library imports first
- Third-party imports second
- Local application imports third
- Organize imports alphabetically within each section
- Avoid wildcard imports (from module import *)

#### Naming Conventions
- `snake_case` for functions and variables
- `CamelCase` for classes
- `UPPER_CASE` for constants
- Private functions start with underscore (e.g., `_private_func()`)

#### Documentation
- Use docstrings for all functions and classes (Google-style recommended)
- All public functions should have docstring including Args, Returns, Raises
- Module-level docstrings should explain the purpose of the module

#### Error Handling
- Use specific exception types rather than bare `except:`
- Include proper error messages in exceptions
- Avoid silent exception handling
- Use `try/except/else/finally` blocks appropriately

#### Type Hints
- Use type hints for function parameters and return values
- Import `typing` module for complex type annotations
- Use `Union`, `Optional`, `List`, `Dict`, etc. for complex types

#### Formatting
- Use consistent spacing around operators: `a = b + c` not `a=b+c`
- Place spaces after commas in function calls
- Break long lines with backslash or parentheses
- Use blank lines to separate logical sections of code

#### Examples
```python
def example_function(param1: str, param2: int) -> bool:
    """Example function with type hints.
    
    Args:
        param1: Description of param1
        param2: Description of param2
        
    Returns:
        True if successful, False otherwise
        
    Raises:
        ValueError: If param1 is invalid
    """
    if not isinstance(param1, str):
        raise ValueError("param1 must be a string")

    return param2 > 0
```

## Cursor/Copilot Rules

No specific Cursor rules or Copilot instructions found in the repository structure.