# Gossip-Simulator

Implemented Gossip algorithm and Push-Sum algorithm on various topologies in Scala using akka. Topologies are Full Network, Line, 3D network, Imperfect 3D networks. For Gossip algorithm we started a rumor, spread it using respective topology to all nodes. Each node keeps track of how many times it heard the rumor and algorithm terminates after the rumor is heard 10 times by all the nodes. For Push-Sum algorithm, we initiated two variables, sum s and weight w. While transmitting rumor we kept track of these variables and difference in their ratio. When the Sum estimate ratio s/w didn’t change more than 10-10 in three consecutive rounds we terminated our actors and our algorithm.  
Sample Input examples:
1000 line gossip, 800 full gossip, 512 3D push-sum, 64 imp3D push-sum  
