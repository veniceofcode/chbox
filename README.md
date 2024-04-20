# WIP


## Status

### Get host info
```
 hostnamectl
   Static hostname: (unset)                         
Transient hostname: dhcp-10-26-67-18
         Icon name: computer-desktop
           Chassis: desktop 🖥️
        Machine ID: 669a3114eb9b417dba42c7b6948f2013
           Boot ID: 580cbd7c1df44008910c39a1dc6028b2
  Operating System: CentOS Stream 9                 
       CPE OS Name: cpe:/o:centos:centos:9
            Kernel: Linux 5.14.0-435.el9.x86_64
      Architecture: x86-64
   Hardware Vendor: OnLogic
    Hardware Model: HX500
  Firmware Version: Z01-0002A034

```
### Get  containers info

```
podman ps -a

CONTAINER ID  IMAGE                                          COMMAND               CREATED        STATUS                  PORTS                   NAMES
96c799b72e72  localhost/podman-pause:4.9.4-dev-1710930166                          6 minutes ago  Up 6 minutes                                    1bf5e4561f80-service
c453a4dac0f2  localhost/podman-pause:4.9.4-dev-1710930166                          6 minutes ago  Up 6 minutes                                    229308b4cf91-infra
3335eb7a1125  docker.io/library/postgres:16                  postgres              6 minutes ago  Up 6 minutes                                    minichris-postgres-pod-postgres
6c02c404c0e0  localhost/podman-pause:4.9.4-dev-1710930166                          6 minutes ago  Up 6 minutes                                    bdc1b8ef7a61-infra
48ce0c77c039  docker.io/library/rabbitmq:3                   rabbitmq-server       6 minutes ago  Up 6 minutes                                    minichris-rabbitmq-pod-rabbitmq
95d6dd12fdf9  localhost/podman-pause:4.9.4-dev-1710930166                          6 minutes ago  Up 6 minutes            0.0.0.0:8000->8000/tcp  8542d9b11ad4-infra
b1c4b9415890  ghcr.io/fnndsc/cube:5.0.0                      gunicorn -b 0.0.0...  6 minutes ago  Up 6 minutes (healthy)  0.0.0.0:8000->8000/tcp  minichris-cube-pod-server
2b9b6c1d1290  ghcr.io/fnndsc/cube:5.0.0                                            6 minutes ago  Up 6 minutes (healthy)  0.0.0.0:8000->8000/tcp  minichris-cube-pod-cube-worker
7d04c669be68  ghcr.io/fnndsc/cube:5.0.0                                            6 minutes ago  Up 6 minutes (healthy)  0.0.0.0:8000->8000/tcp  minichris-cube-pod-cube-worker-periodic
627d5a0407e7  ghcr.io/fnndsc/cube:5.0.0                                            6 minutes ago  Up 6 minutes (healthy)  0.0.0.0:8000->8000/tcp  minichris-cube-pod-cube-celery-beat
8402a963d316  localhost/podman-pause:4.9.4-dev-1710930166                          6 minutes ago  Up 6 minutes            0.0.0.0:8020->3000/tcp  6962c7b33b10-infra
cb065dff1de2  ghcr.io/fnndsc/chris_ui:20231003.270-01f1a863  sirv --host --sin...  6 minutes ago  Up 6 minutes            0.0.0.0:8020->3000/tcp  minichris-chrisui-pod-chrisui
1c954beb1e56  localhost/podman-pause:4.9.4-dev-1710930166                          6 minutes ago  Up 6 minutes                                    90142358b529-infra
a022fa0208fc  ghcr.io/fnndsc/pfcon:5.2.2                     gunicorn --bind 0...  6 minutes ago  Up 6 minutes                                    minichris-pfcon-pod-pfcon
1df63e093333  ghcr.io/fnndsc/pman:6.0.1                      gunicorn --bind 0...  6 minutes ago  Up 6 minutes                                    minichris-pfcon-pod-pman

```
