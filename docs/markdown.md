## Code Block

- https://squidfunk.github.io/mkdocs-material/reference/code-blocks/

__JSON__

```json
{
    "key": "value"
}
```

__YAML__

```yaml
site_name: Mkdocs Example
site_url: https://example.com/
nav:
  - Home: index.md
  - About: about.md
# theme: readthedocs
theme:
  name: material
```

__Python__

``` py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```


## Table

```md
Header | Header
------ | ------
Cell   | Cell
Cell   | Cell
```

Header | Header
------ | ------
Cell   | Cell
Cell   | Cell


Columns can be aligned to the right with --: and centered with :--:.

```md
Center | Right
:----: | ----:
Cell   | Cell
Cell   | Cell
```

Center | Right
:----: | ----:
Cell   | Cell
Cell   | Cell

## Images

```md
![](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)
```

![](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)


```md
![](assets/googlelogo_color_272x92dp.png)

```

![](assets/googlelogo_color_272x92dp.png)
