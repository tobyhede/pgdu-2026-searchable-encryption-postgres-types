# Two details that matter

| Choice | Why |
| --- | --- |
| **Not** `STRICT` | `STRICT` returns NULL on NULL input and never calls the function |
| `LANGUAGE plpgsql` | Opaque to SQL-function inlining |

The blocker raises **when evaluated**.
