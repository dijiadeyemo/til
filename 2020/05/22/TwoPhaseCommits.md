# Two-Phase Commits

**Author** : Diji

## Notes
This is an approach for implementing a distributed database transactions

Phases
* Prepare phase: The initiating node, called the global coordinator, asks participating nodes other than the commit point site to promise to commit or roll back the transaction, even if there is a failure. If any node cannot prepare, the transaction is rolled back.
* Commit phase: If all participants respond to the coordinator that they are prepared, then the coordinator asks the commit point site to commit. After it commits, the coordinator asks all other nodes to commit the transaction.
* Forget phase: The global coordinator forgets about the transaction.

## Links
https://docs.oracle.com/cd/B28359_01/server.111/b28310/ds_txns003.htm#ADMIN12223