root@dash:/home/sergey# /opt/packer/packer build /tmp/image_2.json
<br/>yandex: output will be in this color.
<br/>
<br/>==> yandex: Creating temporary RSA SSH key for instance...
<br/>==> yandex: Using as source image: fd8l336b2tdh3m5ijddn (name: "debian-11-v20250224", family: "debian-11")
<br/>==> yandex: Use provided subnet id e2l5e70l9boivd7p6mi1
<br/>==> yandex: Creating disk...
<br/>==> yandex: Creating instance...
<br/>==> yandex: Waiting for instance with id epdibs5gjd3cnhj307pm to become active...
<br/>    yandex: Detected instance IP: 89.169.173.9
<br/>==> yandex: Using SSH communicator to connect: 89.169.173.9
<br/>==> yandex: Waiting for SSH to become available...
<br/>==> yandex: Connected to SSH!
<br/>==> yandex: Provisioning with shell script: /tmp/packer-shell4003396882
<br/>    yandex: Get:1 http://security.debian.org bullseye-security InRelease [27.2 kB]
<br/>    yandex: Get:2 http://mirror.yandex.ru/debian bullseye InRelease [116 kB]
<br/>    yandex: Get:3 http://mirror.yandex.ru/debian bullseye-updates InRelease [44.1 kB]
<br/>    yandex: Get:4 http://mirror.yandex.ru/debian bullseye-backports InRelease [49.0 kB]
<br/>    yandex: Get:5 http://security.debian.org bullseye-security/main Sources [239 kB]
<br/>    yandex: Get:6 http://security.debian.org bullseye-security/main amd64 Packages [350 kB]
<br/>    yandex: Get:7 http://security.debian.org bullseye-security/main Translation-en [227 kB]
<br/>    yandex: Get:8 http://mirror.yandex.ru/debian bullseye/main Sources [8,500 kB]
<br/>    yandex: Get:9 http://mirror.yandex.ru/debian bullseye/main amd64 Packages [8,066 kB]
<br/>    yandex: Get:10 http://mirror.yandex.ru/debian bullseye/main Translation-en [6,235 kB]
<br/>    yandex: Get:11 http://mirror.yandex.ru/debian bullseye/main all Contents (deb) [31.3 MB]
<br/>    yandex: Get:12 http://mirror.yandex.ru/debian bullseye/main amd64 Contents (deb) [10.3 MB]
<br/>    yandex: Get:13 http://mirror.yandex.ru/debian bullseye-updates/main Sources [7,908 B]
<br/>    yandex: Get:14 http://mirror.yandex.ru/debian bullseye-updates/main amd64 Packages [18.8 kB]
<br/>    yandex: Get:15 http://mirror.yandex.ru/debian bullseye-updates/main Translation-en [10.9 kB]
<br/>    yandex: Get:16 http://mirror.yandex.ru/debian bullseye-updates/main amd64 Contents (deb) [88.3 kB]
<br/>    yandex: Get:17 http://mirror.yandex.ru/debian bullseye-updates/main all Contents (deb) [27.3 kB]
<br/>    yandex: Get:18 http://mirror.yandex.ru/debian bullseye-backports/main Sources [376 kB]
<br/>    yandex: Get:19 http://mirror.yandex.ru/debian bullseye-backports/main amd64 Packages [403 kB]
<br/>    yandex: Get:20 http://mirror.yandex.ru/debian bullseye-backports/main Translation-en [344 kB]
<br/>    yandex: Get:21 http://mirror.yandex.ru/debian bullseye-backports/main amd64 Contents (deb) [1,133 kB]
<br/>    yandex: Get:22 http://mirror.yandex.ru/debian bullseye-backports/main all Contents (deb) [4,672 kB]
<br/>    yandex: Fetched 72.6 MB in 20s (3,719 kB/s)
<br/>    yandex: Reading package lists...
<br/>    yandex: -- install htop
<br/>    yandex: Reading package lists...
<br/>    yandex: Building dependency tree...
<br/>    yandex: Reading state information...
<br/>    yandex: htop is already the newest version (3.0.5-7).
<br/>    yandex: 0 upgraded, 0 newly installed, 0 to remove and 5 not upgraded.
<br/>    yandex: -- install tmux
<br/>    yandex: Reading package lists...
<br/>    yandex: Building dependency tree...
<br/>    yandex: Reading state information...
<br/>    yandex: The following additional packages will be installed:
<br/>    yandex:   libevent-2.1-7 libutempter0
<br/>    yandex: The following NEW packages will be installed:
<br/>    yandex:   libevent-2.1-7 libutempter0 tmux
<br/>    yandex: 0 upgraded, 3 newly installed, 0 to remove and 5 not upgraded.
<br/>    yandex: Need to get 560 kB of archives.
<br/>    yandex: After this operation, 1,362 kB of additional disk space will be used.
<br/>    yandex: Get:1 http://mirror.yandex.ru/debian bullseye/main amd64 libevent-2.1-7 amd64 2.1.12-stable-1 [188 kB]
<br/>    yandex: Get:2 http://mirror.yandex.ru/debian bullseye/main amd64 libutempter0 amd64 1.2.1-2 [8,960 B]
<br/>    yandex: Get:3 http://mirror.yandex.ru/debian bullseye/main amd64 tmux amd64 3.1c-1+deb11u1 [363 kB]
<br/>==> yandex: debconf: unable to initialize frontend: Dialog
<br/>==> yandex: debconf: (Dialog frontend will not work on a dumb terminal, an emacs shell buffer, or without a controlling terminal.)
<br/>==> yandex: debconf: falling back to frontend: Readline
<br/>==> yandex: debconf: unable to initialize frontend: Readline
<br/>==> yandex: debconf: (This frontend requires a controlling tty.)
<br/>==> yandex: debconf: falling back to frontend: Teletype
<br/>==> yandex: dpkg-preconfigure: unable to re-open stdin:
<br/>    yandex: Fetched 560 kB in 6s (99.3 kB/s)
<br/>    yandex: Selecting previously unselected package libevent-2.1-7:amd64.
<br/>    yandex: (Reading database ... 34367 files and directories currently installed.)
<br/>    yandex: Preparing to unpack .../libevent-2.1-7_2.1.12-stable-1_amd64.deb ...
<br/>    yandex: Unpacking libevent-2.1-7:amd64 (2.1.12-stable-1) ...
<br/>    yandex: Selecting previously unselected package libutempter0:amd64.
<br/>    yandex: Preparing to unpack .../libutempter0_1.2.1-2_amd64.deb ...
<br/>    yandex: Unpacking libutempter0:amd64 (1.2.1-2) ...
<br/>    yandex: Selecting previously unselected package tmux.
<br/>    yandex: Preparing to unpack .../tmux_3.1c-1+deb11u1_amd64.deb ...
<br/>    yandex: Unpacking tmux (3.1c-1+deb11u1) ...
<br/>    yandex: Setting up libevent-2.1-7:amd64 (2.1.12-stable-1) ...
<br/>    yandex: Setting up libutempter0:amd64 (1.2.1-2) ...
<br/>    yandex: Setting up tmux (3.1c-1+deb11u1) ...
<br/>    yandex: Processing triggers for libc-bin (2.31-13+deb11u11) ...
<br/>    yandex: -- success
<br/>==> yandex: Stopping instance...
<br/>==> yandex: Deleting instance...
<br/>    yandex: Instance has been deleted!
<br/>==> yandex: Creating image: debian-11-docker-htop-tmux
<br/>==> yandex: Waiting for image to complete...
<br/>==> yandex: Success image create...
<br/>==> yandex: Destroying boot disk...
<br/>    yandex: Disk has been deleted!
<br/>Build 'yandex' finished after 2 minutes 22 seconds.
<br/>
<br/>==> Wait completed after 2 minutes 22 seconds
<br/>
<br/>==> Builds finished. The artifacts of successful builds are:
<br/>--> yandex: A disk image was created: debian-11-docker-htop-tmux (id: fd8ioocp5labkvvr45og) with family name
<br/>root@dash:/home/sergey#
<br/>
<br/>
<br/>-----------
<br/>
<br/>Linux compute-vm-2-2-20-ssd-1741374949929 5.10.0-19-amd64 #1 SMP Debian 5.10.149-2 (2022-10-21) x86_64
<br/>
<br/>The programs included with the Debian GNU/Linux system are free software;
<br/>the exact distribution terms for each program are described in the
<br/>individual files in /usr/share/doc/*/copyright.
<br/>
<br/>Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
<br/>permitted by applicable law.
<br/>Last login: Fri Mar  7 19:26:34 2025 from 95.24.151.55
<br/>sergey_gpb@compute-vm-2-2-20-ssd-1741374949929:~$
