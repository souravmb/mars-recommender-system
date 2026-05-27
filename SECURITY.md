# Security Policy

## Scope

This is an academic research repository containing a Jupyter Notebook, a written report, and repository metadata. It does **not** include:

- A web server, API, or any deployed service
- User authentication or personal data storage
- Network-facing code or infrastructure

The primary security surface is the **notebook execution environment** (third-party Python dependencies) and any **data files** downloaded separately from Harvard Dataverse.

---

## Supported Versions

| Version | Status |
|---------|--------|
| `main` branch | ✅ Actively maintained |
| Older commits / forks | ❌ Not supported |

---

## Reporting a Vulnerability

If you discover a security issue — for example, a malicious dependency, a compromised notebook cell, or a supply-chain concern — please **do not open a public GitHub Issue**.

Instead, report it privately by:

1. Opening a **GitHub Security Advisory** via the **Security** tab of this repository (`Security → Advisories → New draft security advisory`), or
2. Contacting the maintainers directly through GitHub (`@souravmb` or `@kashyapramakrishnan`).

Please include:
- A clear description of the vulnerability
- Steps to reproduce, if applicable
- The potential impact
- Any suggested mitigation

We aim to acknowledge reports within **72 hours** and to resolve confirmed issues within **14 days**.

---

## Dependency Security

All dependencies are listed in `requirements.txt`. We recommend:

```bash
pip install pip-audit
pip-audit -r requirements.txt
```

to scan for known vulnerabilities in the dependency tree before running the notebook.

---

## Data Security

The MARS dataset (downloaded separately from Harvard Dataverse) contains anonymised user IDs and watch percentages. It does **not** contain personally identifiable information (PII) per the dataset authors' documentation. Do not attempt to de-anonymise users.

---

## Disclaimer

This project is provided for academic and research purposes only. The maintainers make no warranty regarding security for use cases beyond the intended scope above.
