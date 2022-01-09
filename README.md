# Docker Compose Testnet for Polygon-SDK

# Booting the network is very simple
```
docker compose up
```

# Connecting to metamask to access account with premined tokens
Add a new network to metamask with these settings:
```
RPC URL: http://localhost:31338/
Chain ID: 100
```

Import account to metamask with this private key:
```
425efa3122a9d1036b581e7752538925051abfba9de95461db3cb26693aceff7
```

If it worked you should see a balance of 42m

# How to empty the chain and restart the network from scratch
```
docker compose down
git clean -fdx
```

# TODO:
- Add a block explorer
- Add a faucet script
- Add a reset network script