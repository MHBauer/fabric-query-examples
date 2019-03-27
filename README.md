The smallest working example I could make of some basic interactions with an already set up fabric network.

https://hyperledger-fabric.readthedocs.io/en/release-1.4/build_network.html



1. Start up the default first-network.
2. Start with querying the ledger by `go run query-ledger/main.go`. It
   should pick up the `first-network.yaml` in this directory and print
   out the basic details of the blockchain.

I currently interact mainly with the fabric-chaincode-evm, which is a
go chaincode that has a nice invoke that takes only one argument. This
makes a very easy testcase for me, so you will have to adapt to the
default chaincode for first-network.

Beyond querying the ledger, there is an example for interacting with
chaincode in `query-chaincode`/, along with a program that interacts
with both the ledger and the chaincode in one run in `query-both/`.


