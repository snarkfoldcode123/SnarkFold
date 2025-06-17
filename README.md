# SnarkFold

SnarkFold is a novel SNARK-proof aggregation scheme based on the folding scheme proposed in [Nova](https://par.nsf.gov/servlets/purl/10440508). It offers constant aggregated proof size and constant verification time. SnarkFold adopts incrementally verifiable computation (IVC) for proof aggregation. This repository presents primitive results on simulating Groth16 proof aggregation using Nova's codebase.


# Tests 
By default, we enable the `asm` feature of an underlying library (which boosts performance by up to 50\%).

To run an example: (we recommend the release mode to drastically shorten run times):
```text
cargo run --release --example groth16
```


# Results
We are still implementing Groth16 aggregation. Nonetheless, we can provide some primitive results to estimate our cost by integrating 15 operations (simulating 3 G_1 and 1 G_T) for augmented Groth16 and integrating 18 operations (simulating 6 G_1 and 1 G_T) for the committed Groth16 into Nova’s circuit. For augmented Groth16, this results in 27,794 primary circuit constraints and 28,343 secondary circuit constraints. Compared to the original Nova’s circuit (9,989 primary and 10,518 secondary constraints), this incurs 17,805 additional constraints (approximately 15*1100) as expected. For committed Groth16, we have 31,355 primary and 31,904 secondary constraints.

<img width="323" alt="image" src="https://github.com/user-attachments/assets/f67c6b56-f9a8-4ab0-bbff-6ed76ac4ab32" />
