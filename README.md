# seeded_rand

A small helper crate for reproducible "randomness" in Rust.

This is currently only tailored to be used in specific projects.
It hasn't been tested for general applicability.

## Limitations

Since this crate relies on static/global data to manage the PRNG's seed,
it only works reliably if it is included in the dependency tree of the
application binary only once. Otherwise, setting the seed may only affect
parts of the code base.

## License

This project is licensed under the terms of the MIT License,
as well as the Apache 2.0 License.
You are free to choose whichever suits your needs best.
