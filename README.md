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
02ef86b2b568cb206019942d852161aa242e363461aca28169e961e4fc4966eb  pool/main/f/freetube/freetube_0.23.2_amd64.deb  
8a0b34b7d3e7f46e7bdb0e177cc8086f10bf1bd47e0b7c0182a8a5783f8d8814  pool/main/f/freetube/freetube_0.23.2_arm64.deb  
4e9ef09f516703f377aacedb94dc2570f1c395d4312af4f3cf6e7207df8dab9e  pool/main/f/freetube/freetube_0.23.2_armhf.deb  


# Copyright
The FreeTube installer (deb file) is re-distributed in AGPLv3
