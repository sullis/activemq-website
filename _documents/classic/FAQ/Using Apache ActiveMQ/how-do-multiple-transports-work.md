Apache ActiveMQ ™ -- How do multiple transports work 

 [FAQ](/FAQ/index.md) > [Using Apache ActiveMQ](../../FAQ/using-apache-activemq.md) > [How do multiple transports work](../../FAQ/Using Apache ActiveMQ/how-do-multiple-transports-work.md)


### For ActiveMQ 3.x/4.x

The transport a client uses to connect to the broker is just the transport your client uses. So messages the broker sends to your client will be sent over that transport. However the broker can support many transports.

So client A could connect over HTTP and client B could connect over tcp. Messages client A sends via HTTP will be delivered to B using B's transport, tcp.

