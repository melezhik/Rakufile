# Rakufile

Rakufile specification.

Rakufile is a simple Raku modules dependencies specification.

# File content

Rakufile has one or more lines in the following format:

<Module> <zef options>

Where:

* `<Module>` is zef identity, see https://github.com/ugexe/zef#install-identities

* zef cli options, see https://github.com/ugexe/zef

Thus, every line represents one Raku module dependency. Zef options apply for a certain line (module to be installed)


For example:

`$ cat Rakufile`

```
https://github.com/Kaiepi/p6-Kind.git --/test
https://github.com/Kaiepi/p6-Kind.git
```
