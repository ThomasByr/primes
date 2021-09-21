# Prime Generator

1. [Description](#description)
2. [Usage](#usage)

## Description

This is a simple but effective prime number generator. It generates a memoizable iterator enclosing a Vec that grows as needed from an Iterator. That way, the primes are generated in a lazy fashion. ``Cargo.toml`` has no external dependencies.

## Usage

Tweak the ``RANGE`` constant to generate primes up to that number. Compile with

```powershell
cargo build --release
```

and run with

```powershell
cargo run --release
```

**Note** it should take about 0.7s to generate and count primes up to one billion.

```powershell
cargo run --release
    Finished release [optimized] target(s) in 0.01s
     Running `target\release\primes.exe`
[2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]
50847534
Culling composites took 739 milliseconds.
```
