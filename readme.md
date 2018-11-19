# musikui

## Demo

```
$ python musikui.py -i sample_input.md -o sample_output.md
```

- [sample_input.md](sample_input.md)
- [sample_output.md](sample_output.md)

## Requirement
- Python 3.6+

## Configuration
No easy configable interface yet. Please edit the source directly.

```python
def musikui_string(s):
    import re

    pattern  = r'([^\s#\-\[\]\(\)!`\+\|\.\,\:].){1}([^\s#\-\[\]\(\)!`\+\|\.\,\:].){1}'
    after    = r'@@\2'
    new = re.sub(pattern, after, s)

    return new
```

## License
[MIT License](LICENSE)

## Author
[stakiran](https://github.com/stakiran)
