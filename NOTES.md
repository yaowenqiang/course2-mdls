# Managing Docker on Linux Servers

> vagrant plugin install vagrant-parallels

> ps -auxf

> ctr containers ls

> ctr -n moby containers ls

> ctr -n moby image ls

> ctr namespace ls


make containerd as image store

```
"features": {
    "containerd-snapshotter": true
}


```

> systemctl status docker.service

> docker container run  -i -t --name web -p 8888:80 nginx:latest


> ctr -n moby image pull docker.io/library/ubuntu:latest

> ctr -n moby container ls

> ctr -n moby container info 1da13d6de01a783a82d492e5df57e4484f6cf3ac89dbf118084b323c2d96cbd9  | jq

> ctr -n moby -t run nginx:latest foo

> ctr -n moby container rm foo

> ctr -n moby task ls

> ctr -n moby task kill


> ls /run/docker/runtime-runc/moby

> runc --root /run/docker/runtime-runc/moby list


> ps -p pidofcontainers

> runc --root /run/docker/runtime-runc/moby kill 426c4d3c3300b7be6e5ef67731d826d2d860378b59cd72a4e37b0721259c5a95


> kata runtime

> https://github.com/kata-containers/kata-containers

> https://github.com/opencontainers/runtime-spec/blob/main/implementations.md

> https://docs.docker.com/build/buildkit/


> kubelet

CRI-O

> https://containerd.io/scope/


> live-restore


> https://docs.docker.com/reference/cli/dockerd/#configuration-reload-behavior


> https://docs.docker.com/engine/daemon/live-restore/

> docker roadmap

