```
$ export API_URL=https://testnet.ckb.dev/rpc

$ ckb-cli deploy gen-txs --deployment-config pro-depoyment.toml --migration-dir migrations --from-address ckt1qzda0cr08m85hc8jlnfp3zer7xulejywt49kt2rr0vthywaa50xwsqwn630uyd8qx4cgqw2yhna7rw7lkkzwfacmvvxqt --sign-now --info-file info.json
==== Cell transaction ====
[cell] NewAdded , name: dex-lock, old-capacity: 0.0, new-capacity: 12942.0
> old total capacity: 0.0 (CKB) (removed items not included)
> new total capacity: 12942.0 (CKB)
[transaction fee]: 0.00013365
==== DepGroup transaction ====
> old total capacity: 0.0 (CKB) (removed items not included)
> new total capacity: 0.0 (CKB)
Password: 
status: success

$ ckb-cli deploy apply-txs --migration-dir ./migrations --info-file info.json
> [send cell transaction]: 0x7a879924c9ebf3f6c0d697c86df0e68a07496f3a0526dff25cf6d4c6a8906132
cell_tx: 0x7a879924c9ebf3f6c0d697c86df0e68a07496f3a0526dff25cf6d4c6a8906132
dep_group_tx: ~
```
