## Replication 
A _replica set_ in MongoDB is a group of **mongod** processes that maintain the same data set.
A replica set contains several data bearing nodes and optionally one arbiter node.

 Of the data bearing nodes, _one and only one member_ is deemed the primary node, while the other nodes are deemed secondary nodes.
 The primary node receives all write operations. A replica set can have only one primary capable of confirming writes with _{ w: "majority" }_ write concern

###### More info: https://docs.mongodb.com/manual/replication/

