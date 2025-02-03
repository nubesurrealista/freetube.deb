# freetube-apt
Unofficial APT repository for [FreeTube](https://github.com/FreeTubeApp/FreeTube) that will check for updates regularly

EZ update your FreeTube Debian/Ubuntu client

I do this for myself, but if you want to use it, feel free to audit this repo first and you are strongly recommended to do so.

# Install as APT repo manually
```shell
sudo apt remove freetube # if you installed FreeTube through deb file already, uninstall first.
wget -qO- https://ghaaapt.github.io/freetube-apt/freetube-archive-keyring.asc | gpg --dearmor | sudo tee /usr/share/keyrings/freetube-archive-keyring.gpg > /dev/null
echo 'deb [signed-by=/usr/share/keyrings/freetube-archive-keyring.gpg] https://ghaaapt.github.io/freetube-apt/ stable main' | sudo tee /etc/apt/sources.list.d/freetube.list
sudo apt update
sudo apt install freetube -y
```

# Checksum
6d3ca7c2415e0d739ff3140d3368f5f8268d26ee05e514d1969cb86551665775  pool/main/f/freetube/freetube_0.23.1_amd64.deb  
ed130e7d4b72af53808cbec8ae3d90658b1c6ffc66ef71ebf5624aae5220eb3b  pool/main/f/freetube/freetube_0.23.1_arm64.deb  
88b7ea82aad32e7e2495241f1975396babe1bd4c2b5a86537de6cfdb1caa40cc  pool/main/f/freetube/freetube_0.23.1_armhf.deb  


# Copyright
The FreeTube installer (deb file) is re-distributed in AGPLv3
