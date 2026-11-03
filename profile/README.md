# Swift Compositions

Composed Swift building blocks for production systems — Layer 4 of the [Swift Institute](https://github.com/swift-institute) ecosystem.

## What this is

Packages that compose the lower layers into working systems: HTTP and networking, markup and serialization, cryptography and authentication, database connectivity, I/O and filesystem, rendering, observability, and platform integration. Every package builds on [swift-atoms](https://github.com/swift-atoms) (what must exist), [swift-molecules](https://github.com/swift-molecules) (what is built from atoms alone) and [swift-standards](https://github.com/swift-standards) (specification implementations), and carries the same discipline throughout: typed throws end-to-end, strict memory safety, one repo per package.

## Start here

| Package | What it gives you |
|---|---|
| [swift-pdf](https://github.com/swift-compositions/swift-pdf) | PDF document generation from HTML views and Markdown, authored with a result-builder DSL |
| [swift-html](https://github.com/swift-compositions/swift-html) | Type-safe HTML, CSS, and SVG generation, grounded in the WHATWG and W3C specifications |
| [swift-file-system](https://github.com/swift-compositions/swift-file-system) | Typed filesystem operations — scoped handles, atomic writes, zero-copy reads |
| [swift-io-kernel](https://github.com/swift-compositions/swift-io-kernel) | High-performance async I/O executor that isolates blocking syscalls from Swift's cooperative pool |
| [swift-linter](https://github.com/swift-compositions/swift-linter) | SwiftSyntax-based AST linting with SARIF output |

## Browse everything

The [repositories tab](https://github.com/orgs/swift-compositions/repositories) lists every package with its description. Narrow it down:

[http](https://github.com/orgs/swift-compositions/repositories?q=http) · [html](https://github.com/orgs/swift-compositions/repositories?q=html) · [css](https://github.com/orgs/swift-compositions/repositories?q=css) · [svg](https://github.com/orgs/swift-compositions/repositories?q=svg) · [pdf](https://github.com/orgs/swift-compositions/repositories?q=pdf) · [json](https://github.com/orgs/swift-compositions/repositories?q=json) · [sql](https://github.com/orgs/swift-compositions/repositories?q=sql) · [render](https://github.com/orgs/swift-compositions/repositories?q=render) · [logger](https://github.com/orgs/swift-compositions/repositories?q=logger) · [dependencies](https://github.com/orgs/swift-compositions/repositories?q=dependencies)

## How to use a package

Each package is a separate Swift Package Manager package with its own repository — there is no umbrella swift-compositions package:

```swift
dependencies: [
    .package(url: "https://github.com/swift-compositions/swift-html.git", branch: "main")
]
```

See each package's README for current products, traits, and platform support.

## Status

Public alpha. Packages are released repository by repository; APIs may change until first tagged releases.

Maintained by [Coen ten Thije Boonkkamp](https://github.com/coenttb) — contributions welcome via pull request.

## License

Packages use the Apache License 2.0, except the forks [swift-sql](https://github.com/swift-compositions/swift-sql) and [swift-sqlite](https://github.com/swift-compositions/swift-sqlite), which keep their upstream MIT license.
