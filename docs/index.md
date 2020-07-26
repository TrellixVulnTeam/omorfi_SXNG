# Omorfi–Open morphology of Finnish

![open morphology of finnish](https://flammie.github.io/omorfi/omorfi.png)

Omorfi is a free and open source project containing various tools and data for
natural language processing of Finnish based on knowledge driven paradigm.
The main components of this repository are:

1. _a lexical database_ containing hundreds of thousands of words (c.f.
   [lexical statistics](statistics.html))
2. a collection of _conversion scripts_ to convert lexical database into formats
   upstream NLP tools (c.f. [lexical processing](pages/Database-processing))
3. a collection of _utility scripts_ to process Finnish texts on command-line
   (c.f. [usage examples](pages/usage-examples.html))
4. an _autotools setup_ to build and install (or package, or deploy): the
   scripts, the database, and simple APIs / convenience processing tools
5. a collection of relatively [simple APIs](apis/html/) with bindings for a
   selection of programming languages and scripts to apply the NLP tools and
   access the database

The formats we produce are (links to free open source implementations
included):

1. lexc, as processed by [HFST](//hfst.sf.net) and
   [foma](//code.google.com/p/foma), to be used for *morphological analysis*,
   *stemming*, *segmentation*, *natural language generation*, *hyphenation* and
   as a basis for *language models*,
   1. we provide [pre-built automata binaries for each release as a convenient
   download](https://github.com/flammie/omorfi/releases)
2. [apertium](//sf.net/p/apertium), to be used for *machine translation*
    * See [apertium-fin](//github.com/apertium/apertium-fin)
3. [voikko](//voikko.puimula.org), to be used for *spell-checking* and
   *correction* (also experimental _hunspell_ for legacy spell-checking)
4. _kotus-sanalista_, _lexical markup framework_, _tab-separated values_, etc.
   for long and short term storage, intermediate formats.

## Documentation

The most recent version of this documentation is online on github pages at
https://flammie.github.io/omorfi/

### Basics

1. [README](README.html)
1. [Installation](install.html)
1. [Usage examples](usage-examples.html)

### Bindings

If you wish to use omorfi in a serious application you probably found out from
the README that a python or java API is the way to go:

1. [API design](API-design.html)
1. [doxygen apidocs](apis/html/)

### Statistics and generated listings

There's some [semi-automatically generated statistics](statistics.html)
available.

We also have generated documentation for some aspects of database, such as
paradigms or noteworthy words:

1. [Words](lexemes.html), particularly those that are problematic (a FAQ for
   word entries, in a way)
1. [Paradigms](paradigms.html), i.e. inflection patterns
1. [Internal keys and codes](stuff.html)
1. [All forms of *kauppa*](genkau3.html), a retake on old experiment

### Design, historical notes, stuff

Some notes about design and development

1. [Analysis tags](tag-formats.html)
1. [Design "principles" for tags](Tagging-possibilities.html)
1. [Directory layout](Directory-layout.html)
1. [Database structure](Database-processing.html)
1. [Testing](Regression-testing.html)

## Contact

If you want to discuss about omorfi in Finnish or English, the IRC channels
[#omorfi](irc://Freenode/#omorfi) and [#hfst](irc://Freenode/#hfst) on Freenode
are available for immediate chats ([Freenode webchat
here](https://webchat.freenode.net/)). The google group discussion list
omorfi-devel@groups.google.com ([Google groups web interface
here](https://groups.google.com/forum/#!forum/omorfi-devel)) can also be used,
it may require subscription but is very low volume. Suggestions, bug reports,
corrections and new lexical data can be sent using [github's omorfi issue
tracker](//github.com/flammie/omorfi/issues). Pull requests are accepted.

## Alternatives of omorfi

If omorfi doesn’t suit your needs, you may want to try other similar products:
[suomi-malaga](http://voikko.puimula.org) of voikko fame is another
morphological analyser of Finnish. [Grammatical
Framework](http://www.grammaticalframework.org/) also has NLP components for
Finnish, and it’s written in _haskell_.

If you want to use commercial products, there are surely some available
somewhere.

<!-- vim: set ft=markdown -->
