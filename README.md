[![](https://img.shields.io/pypi/v/foliantcontrib.checksources.svg)](https://pypi.org/project/foliantcontrib.checksources/) [![](https://img.shields.io/github/v/tag/foliant-docs/foliantcontrib.checksources.svg?label=GitHub)](https://github.com/foliant-docs/foliantcontrib.checksources)

# CheckSources

CheckSources is a preprocessor that checks the project’s `chapters` for missing and unmentioned files in the sources directory.

## Installation

```bash
$ pip install foliantcontrib.checksources
```

## Usage

To enable the preprocessor, add `checksources` to `preprocessors` section in the project config:

```yaml
preprocessors:
    - checksources
```

You can add a list of unmentioned files that wouldn't throw warnings by `not_in_chapters` option:

```yaml
preprocessors:
    - checksources:
        not_in_chapters:
          - tags.md
```

It is useful if you don't need to add some files to the table of contents.


