
# case: container run
when you run `vault status` in container

```
WARNING! VAULT_ADDR and -address unset. Defaulting to https://127.0.0.1:8200.

Error checking seal status: Get "https://127.0.0.1:8200/v1/sys/seal-status": http: server gave HTTP response to HTTPS client 
```

- Solution: set `export VAULT_ADDR='http://127.0.0.1:8200'` in advance

Root token
- Root token is auto-generated. You can view in container log by `grep "Root Token:"`