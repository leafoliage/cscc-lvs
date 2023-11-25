# Load Balancer

1. Apply sysctl configs specified in *sysctl.conf*
2. Setup a public net interface with *public-interface-config* and a private net interface with *private-interface-config*
3. Install keepalived

```
yum install keepalived
```

4. For master load balancer, configure keepalived with *keepalived-master.conf*; for backups, *keepalived-bakcup.conf*

> firewalld can be disabled for convenience

```
systemctl disable --now firewalld
```
