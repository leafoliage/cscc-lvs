# CSCC LVS

This is a document for how I set up a small-scale LVS. LVSs are made up of load balancers (LB) and real servers (RS). I installed 4 centos VMs on KVM/Qemu as servers, 2 LB and 2 RS. For detailed configuration, please refer to the *load-balancer* and *real-server* directory.

* Environment: CentOS 7, Keepalived v1.3.5
* LVS Implementation: LVS/NAT

### LVS Topology

![LVS_NAT_topo](https://github.com/leafoliage/cscc-lvs/assets/55055783/fb541031-b194-40bc-8163-14347fc999f0)

## How to test this setup

After you've installed the servers and applied the configs, open `192.168.122.100` in your browser. Then open it in another machine. If different content was set on the RSs, you would see different contents on different machines, indicating that load balancing is working.
