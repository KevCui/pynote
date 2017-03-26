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
usage: note [-h] [-i ID] [-f FILTER] [-t TEMPLATE] [-d] [text [text ...]]

positional arguments:
  text                  input text

optional arguments:
  -h, --help            show this help message and exit
  -i ID, --remove ID    open note with id
  -f FILTER, --filter FILTER
                        filter display result
  -t TEMPLATE, --template TEMPLATE
                        use template
  -d, --debug           active debug log
```

### Example
* Create new note *post* with template *blog*:

```~$ note post -t blog```

* Show all notes and folders:

```~$ note```

* Filter notes by key word *blog*:

```~$ note -f blog```
