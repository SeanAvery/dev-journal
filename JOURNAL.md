# Journal #

## 11/14 ##

Casper Standup:

- History depth in the justification -> time measurement relative to a particular view 
- “Consensus Time” —> put exponential cost on history depth 
- If proposals are not in conflict, they can be collapsed (Re-write system from Vlad)
- not solving flp, rather incentivized to come to consensus
- such economics can disincentivize agent based faults
- propose == rho calculus message combinator
- promote == forwarder combinator
- join == kill combinator 
 
## 11/12 ##

Revewing Casper TFG paper

- fix misspelling in Definition 2.1


## 11/11 ##

Making progress on python_shell <--> webapp for d3 sim 


Gauss Simulation: gaussian(mu, sigma) --> gaussian(mu', sigma) --> gaussian(mu'', sigma) --> ...



## 11/9 ##

Stateless clients: https://ethresear.ch/t/the-stateless-client-concept/172

STF(root, block, witness) -> root`



Halting Problem: given a higher representation of instructions it is impossible to tell wether the program ends or runs forever.


Griefing Factor analysis of casper.



Reviewing category theory.


-- morphisms f : a --> b


## 11/7 ##

looking into representing fix point decimals in solidity


trying to understand "weak-subjectivity" -- https://blog.ethereum.org/2014/11/25/proof-stake-learned-love-weak-subjectivity/


long-range attack problem:

- attacker can purchase "old" keys


### cbc casper ###

get cbc casper repo to run! 


running into strange utf8 error in matplotlib


https://github.com/ethereum/cbc-casper/pull/1/ ---> interesting start for d3 viz


## 11/6 ##

devcon is over. time to get back to work.

### solidity-casper ###

starting to port over viper --> solidity casper contract

viper docs ==> https://media.readthedocs.org/pdf/ethereum-viper/latest/ethereum-viper.pdf


need to understand reason for using decimals.


look into byte-slicing + rlp decoding to replicate viper contract in solidity


## 10/18  ##

### bio-token ###
reviewing facenet library, downloading cuda and pytorch. 

### merkle-proof  ###

Goal: fix tx trie 

## 10/17 ##

### Whisper ###

Goal: Relay a message via whisper

## 10/16 ##

Goal: debug findPath null return

Interesting that tx's are stored by index instead of the tx hash.

Common bug when npm install certain crypto packags.

```
sha1-ZX2ISRe+e0o8HyRUzQmaxiHwppU= integrity checksum failed when using sha
```

to fix:

```
The following solved it for me:

rm -rf node_modules

rm package-lock.json

rm -rf ~/.npm

npm install --update-binary --no-shrinkwrap
```

Looking into how to traverse the patricia tree in Zac's verifier lib 


https://github.com/zmitton/eth-proof/blob/master/buildProof.js

## 10/15 ##

### merkle-proof ###


Goal: create merkle tree out of a given blocks tx tree


pretty much going through and copying https://github.com/zmitton/eth-proof


not too bad, use rpc to get txs in a block, map over them and stuff into a patricia tree


Goal: create a comprehensive "proof" from the patricia tree info

Structured a minimum proof that includes block info and stack of nodes necessary to construct merkle branch up to root. 
Need to make sure sufficient proof info.


Goal: verify tx proof 

... I need to learn more about patricia trees. --> studying up on yellow paper def.


https://ethereum.stackexchange.com/questions/6415/eli5-how-does-a-merkle-patricia-trie-tree-work

https://stackoverflow.com/questions/14708134/what-is-the-difference-between-trie-and-radix-trie-data-structures

https://easythereentropy.wordpress.com/2014/06/04/understanding-the-ethereum-trie/


### bio-coin ###

Goal: pull in youtube data set into python

Downloading tar containing csv data and videos 25 GB's! (taking 2 hours). 
Interesting to think about handeling large data sets. Do I push data into Github?
Nope, max push of 100 MB...


