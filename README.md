# SafetySeal

**Local-first safety inspection, incident, near-miss, and toolbox talk evidence sealer for field operators.**

Offline. Deterministic. Pay once. Compatible with QuantumGuard CONTRACT-v1 and the Operator Pages suite.

## Why SafetySeal?

Undocumented inspections, disputed near-misses, missing toolbox talks, and "we never saw that hazard" claims create liability. Without contemporaneous, verifiable records of what was inspected, by whom, findings, corrective actions, and attendees, defense fails.

SafetySeal captures structured safety records (type, location, inspector, findings, severity, actions, attendees, media hashes) and seals them into a client-verifiable QuantumGuard evidence bundle.

- No SaaS. No subscription. Runs completely offline after key setup.
- Clients, owners, or auditors verify with free QuantumGuard verifier (`qg verify`).
- Deterministic: same inputs → same sealed pack.
- Pairs with DailySeal, DeliverySeal, PermitSeal, and the rest of the Operator Pages suite.

## Quick Start

```bash
pip install cryptography

python3 src/safetyseal.py --demo
python3 src/safetyseal.py --json samples/inspection-001.json --out sealed-safety.json
```

Verify:
```bash
qg verify sealed-safety.json
```
Expected: **PASS**.

## What you can sell

| SKU       | Price | Includes                                      |
|-----------|-------|-----------------------------------------------|
| Operator  | $59   | CLI + sample templates + key setup guide + 1-year email support |
| Command   | $169  | + batch mode + CSV/HTML export + reseller rights |
| Agency    | $449  | + white-label + multi-site key management |

**Buy Operator Pack (test mode):** https://buy.stripe.com/test_5kQeVc951gRG1T2dcYew808  
Contact danpennic@gmail.com for production / other SKUs.  
Repo: https://github.com/danpennic-sys/safetyseals

Source free under Apache-2.0 OR MIT. Commercial packs sold separately.

## License

Apache-2.0 OR MIT
