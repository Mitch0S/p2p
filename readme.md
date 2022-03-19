*Python2Python Network*

_How does it work?_
Connecting
1. A new node is started and pointed towards an already-running node.
2. The node that recieves this request adds the IP of the new node to the list
3. The node that recieves the request then propagates the changes in the node list to all other IPs in that list
4. The node that recieves the request then returns a list of all IPs already on the network.
    b. At this point, all other nodes should have the updated list of IPs in the network
    c. The newly-connected node has a list of all other IPs on the network
    
 
