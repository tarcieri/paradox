# Paradox

An experimental language for verifiable computation using zero-knowledge proofs.

## What is Paradox?

This project is an experiment which attempts to add a high-level programming
language interface to [Bellman], a library for building zkSNARKS implemented
in Rust. Like Bellman, the Paradox compiler is also implemented in Rust.

The goal of Paradox is to allow use of Bellman without knowledge of the Rust
language itself. Instead, Paradox uses Bellman to build a constraint system
which proves a program written in Paradox has been executed correctly.

Ideally Paradox will not be coupled to Bellman specifically, but be able to
target any [rank-1 constraint system]. However, Paradox also aims to make it
possible to access "gadgets" which are unique to Bellman or other hypothetical
Paradox backends which provide things like group operations on elliptic curves,
hash functions, and symmetric encryption.

[Bellman]: https://blog.z.cash/bellman-zksnarks-in-rust/
[rank-1 constraint system]: https://medium.com/@VitalikButerin/quadratic-arithmetic-programs-from-zero-to-hero-f6d558cea649

## License

Copyright (C) 2018 Tony Arcieri

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
