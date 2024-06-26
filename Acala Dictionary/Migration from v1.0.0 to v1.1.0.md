# Migration from v1.0.0 to v1.1.0
```
Old project: Qmarrhgrpqw5VK71rMtb4GARpPvq8ajMjAqnjnWZFLV61N
New project: QmUj8yYCE1YU5UNdtm4q4di4GBDEAmL8vprSRWVGrYeEFm
```


## Upgrade instructions
 1) Stop old project from coordinator (`Qmarrhgrpqw5VK71rMtb4GARpPvq8ajMjAqnjnWZFLV61N`)

```
docker container rm -f query_qmarrhgrpqw5vk7 && docker container rm -f node_qmarrhgrpqw5vk7
```

 2) Execute query.

```
docker exec indexer_db psql -U postgres -c "ALTER SCHEMA schema_qmarrhgrpqw5vk7 RENAME TO schema_qmuj8yyce1yu5un;"

```

 3) Run new project from coordinator (`QmUj8yYCE1YU5UNdtm4q4di4GBDEAmL8vprSRWVGrYeEFm`)

#### RAW Upgrade command. For Native requests.
`ALTER SCHEMA schema_qmarrhgrpqw5vk7 RENAME TO schema_qmuj8yyce1yu5un;`


___
### Setup your own indexer:

[https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md](https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md)

### Projects Updates Alerts channel:

[https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD](https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD)

### Subquery Indexers Monitoring:

[https://t.me/subquery_eagle_eye_bot](https://t.me/subquery_eagle_eye_bot)
