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
1485a55da49f4c8e2a342924fb31db94b38a3a4972e5ce815033d1fac9341192  pool/main/f/freetube/freetube_0.23.0_amd64.deb  
1b2ee96b130558a09df77b91084d335c75f6f5767d22035dd370225f98ca4684  pool/main/f/freetube/freetube_0.23.0_arm64.deb  
559e72fc7490fd5d1253f4633e23490da9de10da31803919d07dc66f69c49ca3  pool/main/f/freetube/freetube_0.23.0_armhf.deb  


# Copyright
The FreeTube installer (deb file) is re-distributed in AGPLv3
