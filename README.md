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
01120e2f039a179cdd342a55cab9608112d31497b80a5ef364da74d73e9fc18e  pool/main/f/freetube/freetube_0.23.4_amd64.deb  
c69ef8d6535986501a41edb2fab16a2618edd7b97ce0d3e19d658b60d916b25a  pool/main/f/freetube/freetube_0.23.4_arm64.deb  
641a49ac8e55a978543f8efd0579f2a988946f425c6d541c4770b93cf7156cb3  pool/main/f/freetube/freetube_0.23.4_armhf.deb  


# Copyright
The FreeTube installer (deb file) is re-distributed in AGPLv3
