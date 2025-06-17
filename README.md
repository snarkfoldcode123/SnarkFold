# SnarkFold

SnarkFold is a novel SNARK-proof aggregation scheme based on the folding scheme proposed in [Nova](https://par.nsf.gov/servlets/purl/10440508). It offers constant aggregated proof size and constant verification time. SnarkFold adopts incrementally verifiable computation (IVC) for proof aggregation. This repository presents primitive results on simulating Groth16 proof aggregation using Nova's codebase.


# Tests 
By default, we enable the `asm` feature of an underlying library (which boosts performance by up to 50\%).

To run an example: (we recommend the release mode to drastically shorten run times):
```text
cargo run --release --example groth16
```


#Results
We provide the primitive results of the constrain numbers and proving time of Groth16 aggregation in the below figure.

<img width="323" alt="image" src="https://github.com/user-attachments/assets/f67c6b56-f9a8-4ab0-bbff-6ed76ac4ab32" />
