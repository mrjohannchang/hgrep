# hgrep

The default outputs of grep isn't good enough for human, hgrep prints more friendly results.
The goal of hgrep is similar to [ack](http://beyondgrep.com/) but hgrep is much more compact and easier to extend.

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
javagrep 'main(.*)'
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
* hgrep
* srcgrep
* cppgrep
* gogrep
* javagrep
* jsgrep
* plgrep
* pygrep
* rbgrep
* xmlgrep
