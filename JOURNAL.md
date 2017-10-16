# Journal #

## 10/15 ##

### merkle-proof ###


Goal: create merkle tree out of a given blocks tx tree


pretty much going through and copying https://github.com/zmitton/eth-proof


not too bad, use rpc to get txs in a block, map over them and stuff into a patricia tree


Goal: create a comprehensive "proof" from the patricia tree info

Structured a minimum proof that includes block info and stack of nodes necessary to construct merkle branch up to root. 
Need to make sure sufficient proof info.


Goal: verify tx proof 





