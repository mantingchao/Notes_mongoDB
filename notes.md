# Replication
- New replica set has a single, primary node.

# Server Sessions (Logical sessions)
- A session is a grouping of related read or write operations that you intend to run sequentially. Sessions enable causal consistency for a group of operations or allow you to execute operations in an ACID transaction. 
https://www.mongodb.com/docs/manual/reference/server-sessions/#server-sessions

# Transaction
- 在 transaction commit 之前所做的事是 unvisible, 直到交易 commit 之後才是 visible
- Run within logical sessions.
![image](https://github.com/mantingchao/Notes_mongoDB/assets/51501170/a23beb59-c06c-43b1-838e-3d675b062e63)
<img width="683" alt="截圖 2023-12-14 21 45 27" src="https://github.com/mantingchao/Notes_mongoDB/assets/51501170/b6d994c4-2da2-4fd7-8a63-5d904c138605">

https://www.mongodb.com/docs/drivers/go/current/fundamentals/transactions/
https://www.prisma.io/dataguide/mongodb/mongodb-transactions
https://www.mongodb.com/docs/drivers/go/current/fundamentals/transactions/
