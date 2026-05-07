# Advanced Topics

## Code blocks

Syntax highlighting works for most languages. Add a title with `title="..."`:

```python title="fibonacci.py"
def fibonacci(n: int) -> int:
    if n <= 1:  # (1)!
        return n
    return fibonacci(n - 1) + fibonacci(n - 2)  # (2)!
```

1. Base case — returns immediately for `0` and `1`.
2. Recursive case — adds the two preceding values.

## Content tabs

=== "Python"

    ```python
    name = "World"
    print(f"Hello, {name}!")
    ```

=== "JavaScript"

    ```js
    const name = "World";
    console.log(`Hello, ${name}!`);
    ```

=== "Bash"

    ```bash
    NAME="World"
    echo "Hello, $NAME!"
    ```

## Tables

| Name       | Type    | Default | Description                       |
|------------|---------|---------|-----------------------------------|
| `site_name`| string  | —       | Name shown in the browser tab     |
| `site_url` | string  | —       | Canonical URL for the site        |
| `theme`    | object  | —       | Theme name and feature flags      |
| `nav`      | list    | —       | Controls sidebar order and labels |

## Custom styling

You can override any CSS by creating `docs/stylesheets/extra.css` and adding it to `mkdocs.yml`:

```yaml
extra_css:
  - stylesheets/extra.css
```

> [!TIP] Keep overrides minimal
> The Material theme covers most use cases. Custom CSS should only be used for **project-specific** branding.
