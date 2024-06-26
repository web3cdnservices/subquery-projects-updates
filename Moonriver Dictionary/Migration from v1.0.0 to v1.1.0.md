# Migration from v1.0.0 to v1.1.0
```
Old project: QmXCr6uZFdY1YcGTa4u6ZieQPXK4VHE1Pjy7CBr7ubFwKR
New project: QmWhwLQA4P6iZv6bmQxUqG5zumNK8KDBwcq8wxN4G213dq
```


## Upgrade instructions
 1) Stop old project from coordinator (`QmXCr6uZFdY1YcGTa4u6ZieQPXK4VHE1Pjy7CBr7ubFwKR`)

```
docker container rm -f query_qmxcr6uzfdy1ycg && docker container rm -f node_qmxcr6uzfdy1ycg
```

 2) Execute query.

```
docker exec indexer_db psql -U postgres -c "ALTER SCHEMA schema_qmxcr6uzfdy1ycg RENAME TO schema_qmwhwlqa4p6izv6;"

```

 3) Run new project from coordinator (`QmWhwLQA4P6iZv6bmQxUqG5zumNK8KDBwcq8wxN4G213dq`)

#### RAW Upgrade command. For Native requests.
`ALTER SCHEMA schema_qmxcr6uzfdy1ycg RENAME TO schema_qmwhwlqa4p6izv6;`


___
### Setup your own indexer:

[https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md](https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md)

### Projects Updates Alerts channel:

[https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD](https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD)

### Subquery Indexers Monitoring:

[https://t.me/subquery_eagle_eye_bot](https://t.me/subquery_eagle_eye_bot)
