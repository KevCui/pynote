---
Title: pynote
Description: :notebook_with_decorative_cover: organize notes easily and simply in terminal
Author: KrazyCavin
Tags: CLI, python, script
created:  25 Mar 2017
---

pynote
==========
pynote is a note organization script, aims to create/modify/find/organize notes easily. As a CLI fan, I tried to find some notes tool in terminal. But I cannot find one which is easily to use. So I decide to create my own tool.

### Requirement
* Python3

### Customization
* Variables below in **note**  can be customized:
```
TIME_FORMAT
TEMPLATE_PATH
EDITOR
```
### How to use
```
usage: note [-h] [-f FOLDER] [-t TEMPLATE] [-d] [text [text ...]]

positional arguments:
  text                  input text

optional arguments:
  -h, --help            show this help message and exit
  -f FOLDER, --folder FOLDER
                        create folder or show files in folder
  -t TEMPLATE, --template TEMPLATE
                        use template
  -d, --debug           active debug log
```

### Example
* Create new *blog* folder:

```~$ note -f blog```

* Create new note *post* with template *blog*:

```~$ note post -t blog```

* Show all notes and folders:

```~$ note```
