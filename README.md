# Python Snippets for Zed IDE

A collection of Python snippets for the [Zed IDE](https://zed.dev) to improve your development speed and productivity.

## Features

This extension provides a comprehensive set of snippets for Python development, including:

- Package and import declarations
- Control structures (if, for, switch)
- Function and method declarations
- Common Go patterns
- HTTP server code
- Testing helpers
- And much more!

## Installation

### Method 1

1. Go to Extensions menu in Zed IDE
2. Search for "python-snippets"
3. Click "Install"

### Method 2

1. Clone this repo:
```
git clone https://github.com/jctosta/python-zed-snippets.git
```
2. Go to Extensions menu in Zed IDE
3. Click "Install Dev Extension"
4. Select the folder you cloned

## Usage

To make snippets appear at the top of the completion list in Zed, add this setting to your Zed settings file:

```json
{
    "snippet_sort_order": "top"
}
```

Start typing the snippet prefix (e.g., `py-def`) in a Python file and press `Tab` to expand the snippet.

## Available Snippets

| Prefix                  | Description                                      |
|-------------------------|--------------------------------------------------|
| `py-im`                 | Import module                                    |
| `py-ifm`                | Import from module                               |
| `py-main`               | `if __name__ == "__main__"` entrypoint           |
| `py-def`                | Function definition                              |
| `py-class`              | Class definition                                 |
| `py-prop`               | Property (getter)                                |
| `py-meth`               | Method definition                                |
| `py-for`                | For loop                                         |
| `py-while`              | While loop                                       |
| `py-if`                 | If statement                                     |
| `py-ifelse`             | If-else statement                                |
| `py-elif`               | Elif block                                       |
| `py-try`                | Try-except block                                 |
| `py-tryf`               | Try-except-finally block                         |
| `py-with`               | With context manager                             |
| `py-ctx`                | Context manager class                            |
| `py-deco`               | Decorator function                               |
| `py-lambda`             | Lambda expression                                |
| `py-lc`                 | List comprehension                               |
| `py-print`              | Print statement                                  |
| `py-fs`                 | F-string                                         |
| `py-logi`               | Logging info message                             |
| `py-logd`               | Logging debug message                            |
| **FastAPI**             |                                                  |
| `py-fastapi-app`        | FastAPI minimal app                              |
| `py-fastapi-route`      | FastAPI route handler                            |
| `py-fastapi-dep`        | FastAPI dependency function                      |
| **Pydantic**            |                                                  |
| `py-pydbase`            | Pydantic BaseModel class                         |
| `py-pydval`             | Pydantic validator                               |
| **Typer**               |                                                  |
| `py-typer-app`          | Typer CLI application setup                      |
| **SQLAlchemy**          |                                                  |
| `py-sa-base`            | SQLAlchemy Base import                           |
| `py-sa-model`           | SQLAlchemy Model                                 |
| `py-sa-session`         | SQLAlchemy session setup                         |
| **unittest**            |                                                  |
| `py-ut`                 | Unittest TestCase                                |
| `py-utmain`             | Unittest main entrypoint                         |
| **pytest**              |                                                  |
| `py-pt`                 | Pytest test function                             |
| `py-ptp`                | Pytest parametrize test                          |
| `py-ptfix`              | Pytest fixture                                   |
| `py-pttable`            | Pytest table-driven test (parametrize)           |
| **Misc**                |                                                  |
| `py-dc`                 | Python dataclass                                 |
| `py-hintf`              | Function with type hints                         |
| `py-doc`                | Function docstring template                      |

## Examples

### Function definition

Type `py-def` and press Tab:

```python
def func(args):
    # Your code here
```

---

### If statement

Type `py-if` and press Tab:

```python
if condition:
    # Your code here
```

---

### Class with property and method

Type `py-class`, then `py-prop`, and `py-meth` inside the class, and press Tab each time:

```python
class MyClass(object):
    def __init__(self, value):
        self._value = value

    @property
    def value(self):
        return self._value

    def my_method(self, arg):
        # Your code here
```

---

### FastAPI minimal app

Type `py-fastapi-app` and press Tab:

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def read_root():
    return {"Hello": "World"}
```

---

### Pytest test function

Type `py-pt` and press Tab:

```python
def test_func():
    # Your test code here
```

---

### Dataclass

Type `py-dc` and press Tab:

```python
from dataclasses import dataclass

@dataclass
class Name:
    field: type
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Author

Carlos Tosta - [jctosta86@gmail.com](mailto:jctosta86@gmail.com)

## Acknowledgments

This extension is inspired by and based on the excellent [Go Snippets for Zed IDE](https://github.com/ayberkgezer/go-zed-snippets) created by [Ayberk Gezer](mailto:ayberkgezer@outlook.com). Many of the snippet ideas, naming conventions, and file structure for this Python extension are derived from that project.

Special thanks to Ayberk Gezer for providing a solid foundation and reference implementation.

## Repository

[https://github.com/jctosta/python-zed-snippets](https://github.com/jctosta/python-zed-snippets)
