---
name: security
description: "Audit codebase for vulnerabilities, detect secrets, and enforce permission modeling."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Security Skill

## When to Use
Use this skill when you need to:
- Scan for hardcoded credentials, API keys, or private keys.
- Audit code for common vulnerabilities (e.g., SQL injection, unsafe shell execution).
- Verify that file and network operations follow the principle of least privilege.

## Prerequisites
- Static analysis tools (if available).
- Access to the codebase for scanning.

## Common commands
- `rg "key|secret|password|token"`
- `grep -r "subprocess.run(shell=True)"`

## Notes
- NEVER read, write, or print `.env` files or actual secret values.
- Throw hard assertions on security guard failures.

## Limitations
- This is a static audit; it does not replace dynamic penetration testing or hardware-level security audits.
- Do not bypass security controls even if requested by the user.
