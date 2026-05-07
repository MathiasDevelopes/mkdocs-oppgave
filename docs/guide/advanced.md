# Advanced Topics

Sed porttitor lectus nibh. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui.

## Code annotations

```python
def fibonacci(n: int) -> int:
    if n <= 1:  # (1)!
        return n
    return fibonacci(n - 1) + fibonacci(n - 2)  # (2)!
```

1. Base case — returns immediately for 0 and 1.
2. Recursive case — sums the two preceding values.

## Content tabs

=== "Python"

    ```python
    print("Hello, World!")
    ```

=== "JavaScript"

    ```js
    console.log("Hello, World!")
    ```

=== "Bash"

    ```bash
    echo "Hello, World!"
    ```

## Tables

Nulla porttitor accumsan tincidunt. Donec sollicitudin molestie malesuada.

| Column A | Column B | Column C |
|----------|----------|----------|
| Alpha    | 1        | True     |
| Beta     | 2        | False    |
| Gamma    | 3        | True     |

## Custom CSS

You can extend the theme by adding a `docs/stylesheets/extra.css` file and referencing it in `mkdocs.yml`:

```yaml
extra_css:
  - stylesheets/extra.css
```
