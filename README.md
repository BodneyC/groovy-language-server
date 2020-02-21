# Purpose of Fork

The purpose of this fork is to add some default classes to the classpath, for example... the groovy jars.

To install the relevant dependencies:

    cd ./mvn-project
    mvn dependency:resolve


If you use only gradle, do the same, but gradle-ish.


# Groovy Language Server

A [language server](https://microsoft.github.io/language-server-protocol/) for [Groovy](http://groovy-lang.org/).

The following language server protocol requests are currently supported:

- completion
- definition
- documentSymbol
- hover
- references
- rename
- signatureHelp
- symbol
- typeDefinition

## Build

To build from the command line, run the following command:

```sh
./gradlew build
```

This will create _build/libs/groovy-language-server-all.jar_.

## Run

To run the language server, use the following command:

```sh
java -jar groovy-language-server-all.jar
```

Language server protocol messages are passed using standard I/O.
