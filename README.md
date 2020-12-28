# A-Number-Theoretic-Approach-for-Fast-Discovery-of-Single-Hop-Wireless-Networks
# The algorithm iterates over the set of network sizes "N". For each network size, 
# the set of potential communication rounds "rounds" is determined, which is a matrix 
# that lists all potential sub-phases per round. For each network relization, a binary 
# transmission matrix "H" is generated randomly (line 20-33) and random link erasure 
# events are simulated (line 34-40, but can be commented out when random link erasures 
# are not considered). For each round, the iteration over the set of all sub-phases is 
# initated (line 47). If interference cancelation is enabled, the matrix "H_active" is 
# as defined in line 49 or it will be commented out when interference cancelation is 
# disabled. From line 50 to line 53, the inactive transmission links for the considered 
# round of "H_active" will be set to 0. From line 54 to 61, the algorithim identifies the
# set of found links, i.e those links, that are active transmission links and no other 
# active transmission link is connected to that same receiver. If all links are found (line 
# 64), the algorithm calculates the number of total rounds needed to find the network topology 
# of the current network relization (line 65) and the average number of rounds over all 
# realizations in line 77.
