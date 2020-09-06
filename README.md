# driftwood
## some logs on the [tide](https://github.com/http-rs/tide)

* [CI ![CI][ci-badge]][ci]
* [API Docs][docs] [![docs.rs docs][docs-badge]][docs]
* [Releases][releases] [![crates.io version][version-badge]][lib-rs]
* [Contributing][contributing]

[ci]: https://github.com/jbr/driftwood/actions?query=workflow%3ACI
[ci-badge]: https://github.com/jbr/driftwood/workflows/CI/badge.svg
[releases]: https://github.com/jbr/driftwood/releases
[docs]: https://docs.rs/driftwood
[contributing]: https://github.com/jbr/driftwood/blob/master/.github/CONTRIBUTING.md
[lib-rs]: https://lib.rs/driftwood
[docs-badge]: https://img.shields.io/badge/docs-latest-blue.svg?style=flat-square
[version-badge]: https://img.shields.io/crates/v/driftwood.svg?style=flat-square

## Installation
```sh
$ cargo add driftwood
```

## Usage
```rust
let mut app = tide::new();
app.with(driftwood::DevLogger); // or ApacheCombinedLogger or ApacheCommonLogger
```

## Safety
This crate uses ``#![deny(unsafe_code)]`` to ensure everything is implemented in
100% Safe Rust.

## License

<sup>
Licensed under either of <a href="LICENSE-APACHE">Apache License, Version
2.0</a> or <a href="LICENSE-MIT">MIT license</a> at your option.
</sup>

<br/>

<sub>
Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in this crate by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.
</sub>
