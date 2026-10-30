# scam-check: a free Claude skill against crypto scams

Paste a suspicious message, link, wallet address or signature request into Claude. The skill checks it for known scam patterns and answers:

- `VERDICT: SAFE`: no red flags found in what you showed
- `VERDICT: CHECK`: something is off, verify first
- `VERDICT: SCAM`: clear scam pattern

It looks for fake "refund" and "compensation" DMs, lookalike domains, poisoned wallet addresses (same first and last characters, different middle), "connect your wallet" traps and risky approvals or signatures.

## Install
1. Download [`scam-check.zip`](../scam-check.zip) (or just [`SKILL.md`](SKILL.md)).
2. In Claude, open Settings, Capabilities, Skills and upload `scam-check.zip`. In Claude Code, put the folder in `~/.claude/skills/`.
3. Paste anything suspicious and ask "is this a scam".

## Safe by design
- Plain text instructions only. No scripts, no network calls, no wallet access.
- It never asks for a seed phrase, private key, password or 2FA code. Anything that does is a scam.

## Not a guarantee
This is a pattern check, not a security product. When in doubt, don't click, don't sign, don't send, and open the official app yourself.
