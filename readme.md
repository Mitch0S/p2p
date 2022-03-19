*Python2Python Network*

_How does it work?_
Connecting
1. A new node is started and pointed towards an already-running node.
2. The node that recieves this request adds the IP of the new node to the list
3. The node that recieves the request then propagates the changes in the node list to all other IPs in that list
4. The node that recieves the request then returns a list of all IPs already on the network.

By the end of the initialisation process, all nodes already on the network have added the IP of the newly connected node in their list of IPs. The newly connected node has retrieved a list of the current IPs in the network
    
 
