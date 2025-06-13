# SnarkFold

SnarkFold is a novel SNARK-proof aggregation scheme based on the folding scheme proposed in [Nova](https://par.nsf.gov/servlets/purl/10440508). It offers constant aggregated proof size and constant verification time. SnarkFold adopts incrementally verifiable computation (IVC) for proof aggregation. This repository presents primitive results on simulating Groth16 proof aggregation using Nova's codebase.


# Tests 
By default, we enable the `asm` feature of an underlying library (which boosts performance by up to 50\%).

To run an example: (we recommend the release mode to drastically shorten run times):
```text
cargo run --release --example groth16
```
