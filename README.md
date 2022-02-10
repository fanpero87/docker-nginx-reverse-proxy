# Nginx Reverse Proxy on Docker

Using Portainer
1. On your Portainer server, go to Stacks and click on "+ Add stack"

![image info](https://files.fongo.ca/api/public/dl/LzeE3DJ3?inline=true)

2. Give it a name, Paste the content of the "docker-compose.yml" file and click on "Deploy the stack"

![image info](https://files.fongo.ca/api/public/dl/fkT96Rdg?inline=true)

These will spin up three (3) ngninx servers and sets up one as Reverse Proxy.

Now, go to the web browser and paste:

```
http://portainer_server_IP:8181/loadbalance
```

Note that since we are using Portainer, we can't use the default port 80 on the nginx servers, that's why we've changed the listening ports on all three servers.
