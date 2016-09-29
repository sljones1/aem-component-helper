## AEM Component CLI
[![NPM](https://nodei.co/npm/aem-component-helper.png)](https://nodei.co/npm/aem-component-helper/)
This Tool was designed to create AEM Skeleton Components via the command line.
It allows for a lot of different options for the Skeleton Component.
### Basic Usage
This command
`aem-component -n C01-headline -g test -l`
Creates this structure
```
C01-headline
|-- _cq_dialog.xml
|-- .content.xml
|-- C01-headline.html
|-- clientlib
    |--.content.xml
    |--css.txt
    |--js.txt
    |--js
    |--css
```
Here is the full list of options:
```
aem-component -h

Usage: index [options]

Options:

  -h, --help           output usage information
  -V, --version        output the version number
  -v, --verbose        verbose output
  -n, --name <s>       set name (required)
  -g, --group <s>      set component group (defaults to .hidden)
  -t, --title [s]      set title (optional)
  -d, --directory [s]  root directory (optional)
  -c, --classic        create classic dialog
  -l, --clientlib     create component clientlib
```
### Config file
There is an option to create an `aem.config` file.
Right now you can specify the directory and group
Example:
```
directory = /apps/project/components/modular/
group = company
```
