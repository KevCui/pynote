# pynote

> Organize notes easily and simply in terminal

pynote is a :notebook_with_decorative_cover: organization script, aims to create/modify/find/organize notes easily. As a CLI fan, I tried to find some notes tool in terminal. But I cannot find one which is easily to use. So I decide to create my own tool.

# Table of Contents

- [Feature](#feature)
- [Requirement](#requirement)
- [Installation](#installation)
- [Customization](#customization)
- [How to use](#how-to-use)
  - [Example](#example)

## Feature

[x] Create folder and notes

[x] Apply a template to a note, while creating or editing it

[x] Show all notes/archived notes

[x] Filter notes by keyword

[x] Choose specific note by id

[x] Archive notes

[x] Remove notes (move to _trash_ folder)

## Requirement

- Python3
- termcolor

## Installation

```bash
pip install -r requirements.txt

```

## Customization

- Variables below in **note** can be customized:

```
TIME_FORMAT: time format to display
TEMPLATE_PATH: path for template files
NOTE_JSON: json file to save note info
PREPEND_TIME: add edit time at the beginning
EDITOR: system editor, if not, set it as vim
```

## How to use

```
usage: note [-h] [-t TEMPLATE] [-i ID] [-f FILTER] [-rm] [-a] [-d]
            [text [text ...]]

positional arguments:
  text                  input text

optional arguments:
  -h, --help            show this help message and exit
  -t TEMPLATE, --template TEMPLATE
                        use template
  -i ID, --id ID        use note id to select a specific note
  -f FILTER, --filter FILTER
                        filter display result
  -rm, --remove         remove a note
  -a, --archive         move note to archive, without parameter to show all
                        archived notes
  -d, --debug           active debug log
```

### Example

- Create new note _post_ with template _blog_:

`~$ note post -t blog`

- Show all notes:

`~$ note`

- Open note by id:

`~$ note -i 1`

- Filter notes by key word _blog_:

`~$ note -f blog`

- Archieve note:

`~$ note -a post`

- Show all archived notes:

`~$ note -a`

- Remove a note by id:

`~$ note -rm -i 1`

---

<a href="https://www.buymeacoffee.com/kevcui" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-orange.png" alt="Buy Me A Coffee" height="60px" width="217px"></a>
