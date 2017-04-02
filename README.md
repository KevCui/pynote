---
Title: pynote
Description: Organize notes easily and simply in terminal
Author: KrazyCavin
Tags: CLI, python, script
created:  25 Mar 2017
---

pynote
==========
pynote is a :notebook_with_decorative_cover: organization script, aims to create/modify/find/organize notes easily. As a CLI fan, I tried to find some notes tool in terminal. But I cannot find one which is easily to use. So I decide to create my own tool.

### Feature
[x] Create folder and notes

[x] Apply a template to a note, while creating or editing it

[x] Show all notes/archived notes

[x] Filter notes by keyword

[x] Choose specific note by id

[x] Archive notes

[x] Remove notes (move to *trash* folder)

### Requirement
* Python3
* termcolor

### Installation
```
pip install -r requirements.txt

```

### Customization
* Variables below in **note**  can be customized:
```
TIME_FORMAT
TEMPLATE_PATH
EDITOR
```
### How to use
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
* Create new note *post* with template *blog*:

```~$ note post -t blog```

* Show all notes:

```~$ note```

* Open note by id:

```~$ note -i 1```

* Filter notes by key word *blog*:

```~$ note -f blog```

* Archieve note:

```~$ note -a post```

* Show all archived notes:

```~$ note -a```

* Remove a note by id:

```~$ note -rm -i 1```
