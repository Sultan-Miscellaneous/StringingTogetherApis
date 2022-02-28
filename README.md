# StringingTogetherApis

Add the following to ~/.ssh/config

```cpp
Host sultan-vm
        User omneya
        HostName 172-105-89-107.ip.linodeusercontent.com
        IdentityFile ~/.ssh/linode

Host sultan-vm-gui
        User omneya
        Compression yes
        LocalForward 5901 127.0.0.1:5901
        LogLevel DEBUG3
        HostName 172-105-89-107.ip.linodeusercontent.com
        IdentityFile ~/.ssh/linode
```



then run:

ssh sultan-vm 

or 

ssh sultan-vm-gui

# To access gui

Download VNC viewer https://www.realvnc.com/en/connect/download/viewer/

Add a new connection

Set ip to localhost:5901

Private key needed and VNC password will be required
