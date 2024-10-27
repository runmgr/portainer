## Portainer

```shell
docker run -d \
--name portainer-portainer-ce-latest \
--restart always \
--pull always \
-v /var/run/docker.sock:/var/run/docker.sock \
-v /var/lib/srv/$USER/docker/portainer/portainer/latest/rootfs/data:/data \
-v /var/lib/srv/$USER/docker/portainer/portainer/latest/rootfs/config:/config \
-p 50031:9443 \
-p 50030:8000 \
portainer/portainer-ce:latest 

```
