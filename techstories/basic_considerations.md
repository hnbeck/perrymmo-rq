# Basic technology considerations

Today, most IT landscape is shaped accordig the paradigma client and server. Microservices, cloud architectures and cloud services have introduced many variants and shades of gray to this paradigma. But the common basic fact is, thats some nodes which we call server host all the data, and clients ask for them. 

# P2P
Many years before, Peer-to-Peer (P2P) networks were much more common. The advantage is that data are distributed over the network. A node can fetch data by multiple ways, and the failure of one node is nearly without consequences. 

In a computer game, especially a MMO where a big game world for the players needs a big amount of bits for the digitial representation, P2P has to be checked for usefulness in technical and user perspective.

# Croquet
The othe thing is replication. The Croquet system invented by Alan Kay et. al. around the year 2000 showed, the a big virtual world can be shared by P2P. The approach was called replicated computing. Instead of sending data, only methods (=computational actions) are sended around. In ths case, every node calculated the data by themselfs, but because this calculation was done in exact the same order and with the same effects lika any other node every node in sum had the exact same data. 

Croquet was implemented in Squeak Smalltalk. I want to know if it is possible to replicated logical queries like in Prolog instead of the method calls in Smalltalk. 

# Rule system
Basic element of the game mechanics are so-called rules. The rules have the form of "IF fact THEN consequence". Rules shall control everything from physics, character development, environment development up to behaviour rules like in any desktop game ("Brettspiel"). Therefore, an Prolog system which can implement rules efficiently and is also a system capable of reflection and meta programming shall be included in the technology stack.


# Requirements

Assuming a "node" is a computational unit for playing Perry MMO like PC, mobile Phone, AR device. Then: 

-  RT01: The network of nodes shall be designed such that a node can be added to the network of nodes or deleted from the network. If added, the new node shall get all updates of the current state of gaming world. If deleted, the last state related to the player associated with the noded shall be saved.
-  RT02: the messages (later the replication) shall build from queries asking for a fact. A Fact can be some data like position of spaceships or planets, but it can also complexer things. If a message is received a query is done.