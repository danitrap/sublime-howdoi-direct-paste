# Paste code from StackOverflow search result directly into Sublime Text 2

Windows compatible :)


<img src="http://azac.pl/out.gif" width="400"/>

Fork of [azac/sublime-howdoi-direct-paste](https://github.com/azac/sublime-howdoi-direct-paste)

Based on [howdoi](https://github.com/gleitz/howdoi).

## Installation

1. Install **howdoi**: `pip install howdoi` (!!!)
2. Clone this repo into `Packages` directory [Sublime Text 2 menu >> Preferences >> Browse Packages...]
```git clone https://github.com/azac/sublime-howdoi-direct-paste```

## Usage

1. write what you need
2. press `cmd+shift+h` (`ctrl-shift-h` on Windows and Linux) 

## Troubleshooting howdoi install
I had troubles with the exe howdoi provides, and decided to fully install it via pip.

### requests was outdated
    pip install requests --upgrade

### lxml was not building

1. I have Python 2.6 that was already installed.
2. I installed mingw32 to C:\programs\mingw\
3. Add mingw32's bin directory to your environment variable: append c:\programs\MinGW\bin; to the PATH
4. Edit (create if not existing) distutils.cfg file located at C:\Python26\Lib\distutils\distutils.cfg to be:

```
[build]
compiler=mingw32
```

source: [ninMonkey on Stack Overflow](http://stackoverflow.com/a/2838827/2999682)

#### error: Unable to find vcvarsall.bat

You can install compiled version [of lxml] from http://www.lfd.uci.edu/~gohlke/pythonlibs/

source: [VolodymyrB on Stack Overflow](http://stackoverflow.com/a/5983696/2999682)
