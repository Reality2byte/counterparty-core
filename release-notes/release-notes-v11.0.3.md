# Release Notes - Counterparty Core v11.0.3 (2025-10-??)

# Upgrading

**Upgrade Instructions:**

To upgrade, download the latest version of `counterparty-core` and restart `counterparty-server`.

With Docker Compose:

```bash
cd counterparty-core
git pull
docker compose stop counterparty-core
docker compose --profile mainnet up -d
```

or use `ctrl-c` to interrupt the server:

```bash
cd counterparty-core
git pull
cd counterparty-rs
pip install -e .
cd ../counterparty-core
pip install -e .
counterparty-server start
```

# ChangeLog

## Bugfixes

- Fix get events by addresses endpoint
- Exclude /v2/addresses/mempool from cache
- Don't cache invalid issuances

## Codebase


## API


## CLI

# Credits

- Ouziel Slama
- Adam Krellenstein
