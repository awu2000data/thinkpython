# Think Python

Source code with fixes and precompiled EPUB of the original [Think Python](http://thinkpython.com) book in Version 2.0.13. Original source code was taken from the published [ZIP-File](http://www.greenteapress.com/thinkpython/thinkpython.tex.zip).

## Installation
Clone this repository:
```shell
$ git clone https://github.com/thii/thinkpython
```

## Usage (OSX)

### Prerequisites

The following commands have to be installed:

    latex sed grep pdftops hevea imagen hacha ebook-convert

`sed` and `grep` are preinstalled on OSX.

You can install `latex` from [MacTex](http://www.tug.org/mactex/). `pdftops` (from `poppler` package), `hevea` and `hacha` (included in `hevea` package) can be installed using Homebrew:
```shell
$ brew update
$ brew install poppler
$ brew install hevea
```

Install `imagen` using `pip`:
```shell
$ pip install imagen
```

Download & install [calibre](http://calibre-ebook.com/download) and make a sym-link for `ebook-convert` command-line:
```shell
$ ln -s /Applications/calibre.app/Contents/MacOS/ebook-convert ~/bin/ebook-convert
$ export PATH=$HOME/bin:$PATH >> ~/.bash_profile
$ source ~/.bash_profile
```

### Making EPUB & MOBI
```shell
$ cd thinkpython
$ make epub
$ make mobi
```

`thinkpython.epub` and `thinkpython.mobi` will be generated in the project's root directory.

Precompiled ebook in EPUB and MOBI format can be downloaded from the following URLs:
- [thinkpython.epub](https://github.com/thii/thinkpython/releases/download/v2.0.13/thinkpython.epub)
- [thinkpython.mobi](https://github.com/thii/thinkpython/releases/download/v2.0.13/thinkpython.mobi)

## License

[Creative Commons Attribution-NonCommercial 3.0 Unported License](http://creativecommons.org/licenses/by-nc/3.0/)
