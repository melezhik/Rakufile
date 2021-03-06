# Rakufile

Rakufile specification.

Rakufile is a simple Raku modules dependencies specification.

# File content

Rakufile has one or more lines in the following format:

```
<Module> <zef options>
```

Where:

* `<Module>` is zef identity, see https://github.com/ugexe/zef#install-identities

* `<zef options>` is zef cli options, see https://github.com/ugexe/zef

Thus, every line represents one Raku module dependency. Zef options apply for a certain line (module to be installed)


For example:

`$ cat Rakufile`

```
Hash::Merge --/test
https://github.com/Kaiepi/p6-Kind.git
```

Comments.

You could use comments here, using  lines starting with `#` symbols:

```
# This module tests fail
Data::Dump --/test
```

# Specification implementation

Rakufile specification is implemented and supported in the following tools:

* Sparrow
* RakuDist
* RakuPlay

