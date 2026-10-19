# The expression index

```sql
CREATE INDEX users_email_eq
ON users USING btree (eql_v3.eq_term(encrypted_email));
```

- Indexes the extracted equality term, not the envelope
- `eq_term` returns a domain over `text`, so the default text btree class applies
