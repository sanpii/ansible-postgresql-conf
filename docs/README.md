# postgresql_conf

Modify the postgresql configuration.

## Requirements

- pg_conftool

## Example Playbook

```yaml
- postgresql_conf:
    key: bonjour
    state: absent

- postgresql_conf:
    key: max_connections
    value: 100
    state: present

- postgresql_conf:
    key: shared_preload_libraries
    value: powa
    state: append
```

## License

MIT
