# Gao Math Lab

A public mathematics research studio for exact numerical experiments, counterexample search, and independently checkable local proofs.

**[Open Gao Math Lab](https://gaomathlab.com/)** — the English-language dashboard works in desktop and mobile browsers without a viewer account.

## What you can inspect

- Collatz starting-integer experiments and saved trajectory records.
- Goldbach prime-pair checks and independent verification of candidate counterexamples.
- Conditional Collatz descent lemmas with downloadable arithmetic certificates.
- A bounded conjecture-and-proof workflow using local rule templates, supported Lean 4 proof templates, and optional literature leads.

Paid AI conjecture generation is disabled unless separately approved and configured. The project does not claim to solve the global Collatz or Goldbach conjectures or to establish the novelty of its local results.

## A small result you can reproduce

Use the accelerated Collatz map `T(n) = n / 2` for even `n`, and `T(n) = (3*n + 1) / 2` for odd `n`.
For `n = 4*q + 1` and `q >= 1`, two steps give:

```text
T(4q + 1) = 6q + 2
T²(4q + 1) = 3q + 1 < 4q + 1
```

This proves a local descent condition for `n >= 5` with `n ≡ 1 (mod 4)`. The boundary `n = 1` follows `1 → 2 → 1` and does not descend strictly. A proof under these assumptions is not a proof for every positive integer.

Read the [verification methods and worked example](https://gaomathlab.com/research-methods/) for the scope of the experiment, independent arithmetic checks, and formal verification statuses.

## Reading the evidence

A finite checked range is numerical evidence. A counterexample search that times out is inconclusive. A Lean proof establishes its encoded formal statement and assumptions. Literature search results are leads for comparison; they do not establish that a result is new.

This repository contains the public project introduction. The running dashboard, current evidence, and research guides are hosted on the project website.
