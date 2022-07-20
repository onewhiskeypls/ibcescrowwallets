# ibcescrowwallets

Just a repo for me to pass around this csv. may upload the go script later, probably not though

## Steps

1. Execute go app per gaiad, osmosisd, junod. 
2. Combine Channels arrays
3. pass through this site https://www.convertcsv.com/json-to-csv.htm
4. ??
5. upload csv file

## finding addresses

find destination channel info:
```
gaiad q ibc channel client-state transfer channel-141 --chain-id 1 --node https://rpc.cosmos.network
```

find escrow address:
```
gaiad q ibc-transfer escrow-address transfer channel-141 --chain-id 1 --node https://rpc.cosmos.network
```

query balances:
```
gaiad q bank balances cosmos1x54ltnyg88k0ejmk8ytwrhd3ltm84xehrnlslf --chain-id 1 --node https://rpc.cosmos.network:443
```
