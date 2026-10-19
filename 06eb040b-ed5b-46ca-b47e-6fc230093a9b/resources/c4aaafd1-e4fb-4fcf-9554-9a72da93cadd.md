# An encrypted envelope

```json
{
  "v": "3",
  "i": { "t": "users", "c": "email" },
  "c": "…ciphertext…",
  "hm": "…keyed equality term…"
}
```

- `c`: ciphertext, never read by the database
- `hm`: HMAC term used for equality
- `v`, `i`: version and identifier
