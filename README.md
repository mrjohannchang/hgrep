# hgrep

The default outputs of grep isn't good enough for human reading.
hgrep prints more friendly results.
The goal of hgrep is similar to [ack](http://beyondgrep.com/)
but with much more compact source.

hgrep accepts the same arguments and regex expression with traditional grep.

## Usage

```sh
hgrep PATTERN
```

E.g.
```sh
hgrep 'hello'
```

**To search only in specific language files**

```sh
LANGUAGEgrep PATTERN
```

E.g.
```sh
javagrep -i 'main(.*)'
```

**To search in all recognized programming language files**

```sh
srcgrep PATTERN
```

E.g.
```sh
srcgrep 'iddqd'
```

## Command list
* hgrep - search in all text files
* srcgrep - search in all programming language files
* cppgrep - search in C and C++ files
* gogrep - search in Go files
* javagrep - search in Java files
* jsgrep - search in JavaScript files
* plgrep - search in Perl files
* pygrep - search in Python files
* rbgrep - search in Ruby files
* xmlgrep - search in XML files

## Installation

Choose one of the following methods.

### From the internet

Paste the below line into your terminal and enter.

```sh
tmpdir="`mktemp -d`" && cd "$tmpdir" && wget -O - https://github.com/changyuheng/hgrep/archive/master.zip > hgrep.zip && unzip hgrep.zip && cd hgrep-master && ./install.sh && cd ; rm -rf "$tmpdir" ; unset tmpdir
```

### From the source

Clone the repository and enter it then execute the installing file to install
to `${HOME}/bin`

```sh
./install
```

Or by yourself

```sh
cp -P *grep DESTINATION
```

## License

Except where otherwise noted, all parts of this software is licensed under the
[MIT license](http://opensource.org/licenses/MIT).

© 2015 Chang Yu-heng
