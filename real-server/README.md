# Real Server

1. Apply sysctl configs specified in *sysctl.conf*
2. Set up network interface with *private-interface-config*
3. Install httpd

```
yum install httpd
systemctl enable --now httpd
```

4. Modify webpage content at /var/www/html/index.html

You can also install any service whichever you want
