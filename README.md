#Python2Python Network

##_How does it work? Connecting_
1. A new node is started and pointed towards an already-running node.
2. The node that recieves this request adds the IP of the new node to the list
3. The node that recieves the request then propagates the changes in the node list to all other IPs in that list
4. The node that recieves the request then returns a list of all IPs already on the network.

> By the end of the initialisation process, all nodes already on the network have added the IP of the newly connected node in their list of IPs. The newly connected node has retrieved a list of the current IPs in the network


    
 
##_How does it work?_
Propagating information
1. When a node makes a new message, it will send it to a set amount of nodes in its IP list.
2. The nodes that recieve the message check if they have already recieved the same message within a set amount of time
3. If they have not recieved the message, they relay the message on to a set amount of nodes within its IP list 
4. If they have already received the message, they completely drop the message and do not relay it to any other nodes.

> When referencing to "a set amount of nodes in it's IP list", I am referencing to any amount, can be all of the IPs in the list, or only 1.
