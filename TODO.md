# TODO List

## Management (Luo Man & Zheng Hongren)
1. Account management (Ask Junlin Liu for help)
  * Cloud providers: AWS, Azure, Huawei, Tencent
  * Apply for an outlook email for this project.
  * Apply for account as cloud users
2. Study Cloud provider v.s. region distribution
3. Study Service model, i.e., how CPU, memory, and network are provisioned.
4. Practice Login method, we suggest to use public key method
5. Check the security policy, i.e., whether certain network traffic can get through
 

## Tunneling (Xiong Dian, ask Yongchao He for help)
1. Practice on a single machine
2. Set up several isolated virtual machines, suggestion: KVM+OVS, or docker+Linux Namespace
3. In each VM, configure IP addresses. Make sure they can ping each other.
4. In each VM, install an OVS
5. Configure a tunnel between two OVSes (e.g., GRE or VxLAN), set up a virtual address on each OVS
6. Make sure OVS can use virtual IP address to ping each other.

## SDN Controller (Mei Zhiyu, ask Fu Qi-An for help)
1. Practice on a single machine
2. Install RYU and mininet
3. Use mininet to build a small network with hosts and switches, and let switches to connect to a local RYU controller
4. Write a l2 learning switch (or Dijkstra Algorithm) on RYU, and test whether hosts can ping each other. 
  * Get toplogy, i.e., a switches neighbors, port connections
  * Compute a path for a packet
  * Compute forwarding tables, i.e., header fields to a switch port
  * Install switching rules

## Measurement (Zheng Hongren & Luo Man)
1. Tools to use: iperf for bandwidth/oscillation; sockperf for RTT; traceroute for path
2. Schedule pairwise measurement (avoid a server sending/receiving with two servers, excluding interference), one of the following approaches
  * Pre-compute pairwise measurement sequence, use CRON to run pre-computed script
  * Build a distributed system to schedule all pairwise measurements iteratively (need to build and debug a distributed system, not considered now)
  * Use a simulator for the approach above, and execute to get a measurement plan, then use CRON to set up the plan.
3. Practice on a single machine
4. Set up several isolated virtual machines, suggestion: KVM+OVS, or docker+Linux Namespace
5. Test the measurement plan in step 2, make sure they work
  

## Routing

## Paper writing
1. Collect literatures
  * Google "Overlay Networks" find recent 20 years paper. 
  * For each paper, check its references and papers with it as a reference
  * Download pdf, name the pdf as "Year_Conference_FirstAuthorLastName_SystemNameOrKeyWords"
2. Build paper writing repository
  * Suggest Overleaf, but no hurry now.
