---
layout: post
title: OCS Inventory & OpenVPN
date: 2021-09-26 02:52:05
---
### **Installation OCS Inventory**

You need to add our repository using the following command

```
$ curl -sS http://deb.ocsinventory-ng.org/pubkey.gpg | sudo apt-key add -
$ echo "deb http://deb.ocsinventory-ng.org/ubuntu/ focal main" | sudo tee /etc/apt/sources.list.d/ocsinventory.list
$ sudo apt update

focal | stable
bionic | oldstable
xenial | backport
Then install the agent using :

$ sudo apt install ocsinventory-agent
```

### Installation OpenVPN for Debian and Ubuntu

Follow these steps in order to install OpenVPN 3 Client on Linux for Debian and Ubuntu:\
\
Open the Terminal by pressing **ctrl + alt + T**\
\
Type the following command into the Terminal:

```
 sudo apt install apt-transport-https
```

 This is done to ensure that your apt supports the https transport. Enter the password as prompted\
\
Type the following command into the Terminal: 

```
sudo wget https://swupdate.openvpn.net/repos/openvpn-repo-pkg-key.pub
```

This will install the OpenVPN repository key used by the OpenVPN 3 Linux packages\
\
Type the following command into the Terminal: 

```
sudo apt-key add openvpn-repo-pkg-key.pub
```

\
Type the following command into the Terminal: 

```
sudo wget -O /etc/apt/sources.list.d/openvpn3.list https://swupdate.openvpn.net/community/openvpn3/repos/openvpn3-$DISTRO.list
```

This will install the proper repository. Replace $DISTRO with the release name depending on your Debian/Ubuntu distribution (the table of release names for each distribution can be found below). In this case, focal is chosen since Ubuntu 20.04 is used\
\
Type the following command into the Terminal: 

```
sudo apt update
```

\
Type the following command into the Terminal: 

```
sudo apt install openvpn3
```