# API Blueprint

<img align="right" alt="API Blueprint logo" height="89" width="100" src="./assets/logo_apiblueprint.png"/>

### API Design for Humans

A powerful high-level API design language for web APIs.

API Blueprint is simple and accessible to everybody involved in the API design
lifecycle.\
Its syntax is concise yet expressive.

## At home on GitHub
API Blueprint language is recognized by GitHub. You can
[search for API Blueprint][search] or use the `apib` language identifier for
[syntax highlighting][gfm].

[search]: https://github.com/search?utf8=%E2%9C%93&q=language%3A%22API+Blueprint%22&type=Repositories&ref=advsearch&l=API+Blueprint&l=

[gfm]: https://help.github.com/articles/github-flavored-markdown/#syntax-highlighting

## Getting started
All it takes to describe an endpoint of your API is to write:

```apib
# GET /message
+ Response 200 (text/plain)

        Hello World!
```

in your favorite plain text editor.

To learn more about the API Blueprint syntax jump directly to the
[API Blueprint Tutorial][tutorial] or take a look at some [examples][].

[tutorial]: Tutorial.md
[examples]: https://github.com/funbox/api-blueprint/tree/master/examples

## Media Type
The media type for API Blueprint is `text/vnd.apiblueprint`.

## Learn more
- [Tutorial][tutorial]
- [Advanced Tutorial][advanced_tutorial]
- [Examples][examples]
- [Glossary of Terms][glossary]
- [Specification][specification]

[advanced_tutorial]: Advanced%20Tutorial.md
[glossary]: Glossary%20of%20Terms.md
[specification]: API%20Blueprint%20Specification.md

## Disclaimer

This repository is a fork of the [API Blueprint specification](https://github.com/apiaryio/api-blueprint) by Apiary.
It includes some changes compared to the original specification, adds new sections, and drops unused ones.

### Reasons for creating a forked version

In FunBox, we created our tools to work with API documentation. You can look at the [@funboxteam/crafter](https://github.com/funbox/crafter)
and [@funboxteam/blueprinter-frontend](https://github.com/funbox/blueprinter-frontend) repositories to get a better understanding of what they are.

These tools are mostly based on the original specification, but some newly implemented features also require changes in the specification.
Unfortunately, our attempts to propose are stuck in conversations (see [request](https://github.com/apiaryio/api-blueprint-rfcs/pull/16)
for adding Resource prototypes).

In order to take the opportunity for independent developing of features we decided to make a fork and support it on our own.

### Differences between the fork and the original specification

* **Dropped support** of Resource model section and Relation section.
* **Resource prototypes** section definition was added. This allows you to set up common responses in one place and reuse them through the documentation.
* **Import** section definition was added. This allows to implement modular documentation and inject APIB files into each other.
* Definitions of **Group, SubGroup and Message** sections were added. This allows to describe non-HTTP interaction in a documentation.
* **Schema Structures** section definition was added. This allows to describe complex data structures directly in JSON Schema format.
* A few other non-significant improvements.

## License
MIT License. See the [LICENSE](https://github.com/funbox/api-blueprint/blob/master/LICENSE) file.

[![Sponsored by FunBox](https://funbox.ru/badges/sponsored_by_funbox_centered.svg)](https://funbox.ru)
