# docker

##  Fedora33 运行docker iamges:
    sudo mkdir /sys/fs/cgroup/systemd
    sudo mount -t cgroup -o none,name=systemd cgroup /sys/fs/cgroup/systemd 
    run -it -v  /home/tf:/home/tf --privileged=true 54b6e0fcedce /bin/bash
    
