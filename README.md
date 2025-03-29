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
66724db6cb021d2fc5809a49deb46fc9ce9c26294733a364f6b6d9b9d2e80932  pool/main/f/freetube/freetube_0.23.3_amd64.deb  
294fdbb0ead58d73add13039c7088c5e277df2489d718ace19a9c09ecc6bd11b  pool/main/f/freetube/freetube_0.23.3_arm64.deb  
136a2030f46c31a52fe35e2a4451cb5bb5a079fc2e96b04d0184b6c682680538  pool/main/f/freetube/freetube_0.23.3_armhf.deb  


# Copyright
The FreeTube installer (deb file) is re-distributed in AGPLv3
