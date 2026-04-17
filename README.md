# Python Snippets for Zed IDE

A collection of Python snippets for the [Zed IDE](https://zed.dev) to improve your development speed and productivity.

## Features

This extension provides a comprehensive set of snippets for Python development, including:

- Package and import declarations
- Control structures (if, for, while, try/except)
- Function and method declarations
- Modern Python features (f-strings, type hints, dataclasses)
- Framework-specific snippets (FastAPI, Pydantic, Typer)
- Database ORM snippets (SQLAlchemy)
- Testing helpers (unittest, pytest)
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

Start typing the snippet prefix (e.g., `def`) in a Python file and press `Tab` to expand the snippet.

## Available Snippets

| Prefix                  | Description                                      |
|-------------------------|--------------------------------------------------|
| `im`                    | Import module                                    |
| `ifm`                   | Import from module                               |
| `main`                  | `if __name__ == "__main__"` entrypoint           |
| `def`                   | Function definition                              |
| `class`                 | Class definition                                 |
| `prop`                  | Property (getter)                                |
| `meth`                  | Method definition                                |
| `for`                   | For loop                                         |
| `while`                 | While loop                                       |
| `if`                    | If statement                                     |
| `ifelse`                | If-else statement                                |
| `elif`                  | Elif block                                       |
| `try`                   | Try-except block                                 |
| `tryf`                  | Try-except-finally block                         |
| `with`                  | With context manager                             |
| `ctx`                   | Context manager class                            |
| `deco`                  | Decorator function                               |
| `lambda`                | Lambda expression                                |
| `lc`                    | List comprehension                               |
| `print`                 | Print statement                                  |
| `fs`                    | F-string                                         |
| `logi`                  | Logging info message                             |
| `logd`                  | Logging debug message                            |
| **FastAPI**             |                                                  |
| `fastapi-app`           | FastAPI minimal app                              |
| `fastapi-route`         | FastAPI route handler                            |
| `fastapi-dep`           | FastAPI dependency function                      |
| **Pydantic**            |                                                  |
| `pydbase`               | Pydantic BaseModel class                         |
| `pydval`                | Pydantic validator                               |
| **Typer**               |                                                  |
| `typer-app`             | Typer CLI application setup                      |
| **SQLAlchemy**          |                                                  |
| `sa-base`               | SQLAlchemy Base import                           |
| `sa-model`              | SQLAlchemy Model                                 |
| `sa-session`            | SQLAlchemy session setup                         |
| **unittest**            |                                                  |
| `ut`                    | Unittest TestCase                                |
| `utmain`                | Unittest main entrypoint                         |
| **pytest**              |                                                  |
| `pt`                    | Pytest test function                             |
| `ptp`                   | Pytest parametrize test                          |
| `ptfix`                 | Pytest fixture                                   |
| `pttable`               | Pytest table-driven test (parametrize)           |
| **Asyncio**             |                                                  |
| `adef`                  | Async coroutine definition                       |
| `atg`                   | Async TaskGroup context manager definition       |
| `amain`                 | Main entrypoint with asyncio.run function        |
| **Misc**                |                                                  |
| `dc`                    | Python dataclass                                 |
| `hintf`                 | Function with type hints                         |
| `doc`                   | Function docstring template                      |

## Examples

### Function definition

Type `def` and press Tab:

```python
def func(args):
    # Your code here
```

---

### If statement

Type `if` and press Tab:

```python
if condition:
    # Your code here
```

---

### Class with property and method

Type `class`, then `prop`, and `meth` inside the class, and press Tab each time:

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

Type `fastapi-app` and press Tab:

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def read_root():
    return {"Hello": "World"}
```

---

### Pytest test function

Type `pt` and press Tab:

```python
def test_func():
    # Your test code here
```

---

### Dataclass

Type `dc` and press Tab:

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
