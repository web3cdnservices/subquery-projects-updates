# Migration from v1.0.0 to v1.1.0
```
Old project: QmUmnKPhcE6JwGMYvY3Yitb5j8qxbQBMxgpkHpVQuXqxDH
New project: QmapQ6cNKPtZE1jkeUp5V6xy7sPSiJiZpoqZcRRtyc4Stq
```


## Upgrade instructions
 1) Stop old project from coordinator (`QmUmnKPhcE6JwGMYvY3Yitb5j8qxbQBMxgpkHpVQuXqxDH`)

```
docker container rm -f query_qmumnkphce6jwgm && docker container rm -f node_qmumnkphce6jwgm
```

 2) Execute query.

```
docker exec indexer_db psql -U postgres -c "ALTER SCHEMA schema_qmumnkphce6jwgm RENAME TO schema_qmapq6cnkptze1j;"

```

 3) Run new project from coordinator (`QmapQ6cNKPtZE1jkeUp5V6xy7sPSiJiZpoqZcRRtyc4Stq`)

#### RAW Upgrade command. For Native requests.
`ALTER SCHEMA schema_qmumnkphce6jwgm RENAME TO schema_qmapq6cnkptze1j;`


___
### Setup your own indexer:

[https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md](https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md)

### Projects Updates Alerts channel:

[https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD](https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD)

### Subquery Indexers Monitoring:

[https://t.me/subquery_eagle_eye_bot](https://t.me/subquery_eagle_eye_bot)
