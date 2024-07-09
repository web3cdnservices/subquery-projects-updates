# Subquery project Nova Wallet - Shiden
####  Nova SubQuery project is indexing the blockchain and provides a convenient API for fetching operation history & analytics data. It is used by the Nova Wallet Feel free to use this API for your app! 💖

Make sure that you add filters and sorting rules to your queries!

Following API & datasource is supported: 📚 Transfers and extrinsics (transactions). Both or either can be fetched, for example: 
```
query {
  historyElements{nodes{transfer extrinsic}}
}
```

✨ Transfer history for additional assets in the network (based on "assets"/"ORML" Substrate pallet): 
```
query {
  historyElements{nodes{assetTransfer}}
}
```

👷‍ Node Operator Instruction
- Rpc can be find at [https://onfinality.io](https://onfinality.io)
- Can leave dictionary empty, it should be automatically filled by the sdk if there are any available.

https://app.subquery.network/explorer/project/0x40/overview
____
#### Deployed At: 2024-07-09T03:03:47
____

## Project type:
`Indexer Project`

## Project category:
``

## Is Project Official?
`Yes`

## Latest release version:
`undefined`

## Latest release hash:
`QmaSboGZLXBDAeiAp4xE67eTLa8Tubno4frm7NFwHc2ciP`



___
### Setup your own indexer:

[https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md](https://github.com/web3cdnservices/subquery-indexer-toolkit/blob/mainnet/README.md)

### Projects Updates Alerts channel:

[https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD](https://github.com/web3cdnservices/subquery-projects-updates/blob/master/README.MD)

### Subquery Indexers Monitoring:

[https://t.me/subquery_eagle_eye_bot](https://t.me/subquery_eagle_eye_bot)