# freetube.deb

Repositorio privado para mi uso personal.

Original de: https://github.com/GHaaAPT/freetube-apt

# Install as APT repo manually
```shell
sudo apt remove freetube # if you installed FreeTube through deb file already, uninstall first.
wget -qO- https://nubesurrealista.github.io/freetube.deb/freetube-archive-keyring.asc | gpg --dearmor | sudo tee /usr/share/keyrings/freetube-archive-keyring.gpg > /dev/null
echo 'deb [signed-by=/usr/share/keyrings/freetube-archive-keyring.gpg] https://nubesurrealista.github.io/freetube.deb/ stable main' | sudo tee /etc/apt/sources.list.d/freetube.list
sudo apt update
sudo apt install freetube -y
```

# Checksum
15f42feb853cde3250c320b2e20f8195fdcf1be549b695914c1e6d90c8541ea4  pool/main/f/freetube/freetube_0.23.6_amd64.deb  
75a9fe67046f3b0d03da71f7f0f8b86c560f77f7b27bb7fe4d57355edc560e87  pool/main/f/freetube/freetube_0.23.5_arm64.deb  
dfe70b60bf03a6302679c543e9263152a20832c7a7bf4943a4e73267b803ae12  pool/main/f/freetube/freetube_0.23.5_armhf.deb  


# Copyright
The FreeTube installer (deb file) is re-distributed in AGPLv3
