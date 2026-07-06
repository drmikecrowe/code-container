# Signed Commits

All git commits must be signed. Never create an unsigned commit.

```bash
# Wrong — unsigned
git commit -m "msg"

# Right — signed
git commit -S -m "msg"
```

If a commit fails because signing is not configured, stop and report it — do
not fall back to an unsigned commit. The user will only skip signing when they
explicitly ask for it (e.g. `--no-gpg-sign`).
