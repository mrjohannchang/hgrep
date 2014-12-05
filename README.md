# hgrep

The default outputs of grep isn't good enough for human.
hgrep prints more friendly results.
The goal of hgrep is similar to [ack](http://beyondgrep.com/)
but hgrep is much more compact and easier to extend.

hgrep accepts the same arguments with traditional grep.

## Usage

```sh
hgrep PATTERN
```

E.g.
```sh
hgrep 'hello'
```

**To search only in specific language file**

```sh
<language_abbreviation>grep PATTERN
```

E.g.
```sh
javagrep -i 'main(.*)'
```

**To search in all recognized languages file**

```sh
srcgrep PATTERN
```

E.g.
```sh
srcgrep 'iddqd'
```

## Command list
* hgrep - search in all text file
* srcgrep - search in all programming language file
* cppgrep - search in C and C++ file
* gogrep - search in Go file
* javagrep - search in Java file
* jsgrep - search in JavaScript file
* plgrep - search in Perl file
* pygrep - search in Python file
* rbgrep - search in Ruby file
* xmlgrep - search in XML file

## Installation

Clone the repository and enter it then execute the installing file to install
to `${HOME}/bin`

```sh
./install
```

Or by yourself

```sh
cp -P *grep DESTINATION
```
