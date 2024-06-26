# Migration from v1.0.0 to v1.0.1
```
Old project: QmVJebjZdWAFmhNYx27NRmJ3YgsP8UN94e9GSRxtCRgSJC
New project: QmaDYnfKZohnH98zZQBxUSgnHKmbmwyA8VAf72EyA2zntC
```


## Upgrade instructions
 1) Stop old project from coordinator (`QmVJebjZdWAFmhNYx27NRmJ3YgsP8UN94e9GSRxtCRgSJC`)

```
docker container rm -f query_qmvjebjzdwafmhn && docker container rm -f node_qmvjebjzdwafmhn
```

 2) Execute query.

```
docker exec indexer_db psql -U postgres -c "ALTER SCHEMA schema_qmvjebjzdwafmhn RENAME TO schema_qmadynfkzohnh98;"

```

 3) Run new project from coordinator (`QmaDYnfKZohnH98zZQBxUSgnHKmbmwyA8VAf72EyA2zntC`)

#### RAW Upgrade command. For Native requests.
`ALTER SCHEMA schema_qmvjebjzdwafmhn RENAME TO schema_qmadynfkzohnh98;`


___
### Setup your own indexer:

[https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md](https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md)

### Projects Updates Alerts channel:

[https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD](https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD)

### Subquery Indexers Monitoring:

[https://t.me/subquery_eagle_eye_bot](https://t.me/subquery_eagle_eye_bot)
