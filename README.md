# OpenCloud
Distributed IAAS
Term Project for Cloud Computing CSG527.

Steps of Installation for Prototype Implementation:

**Ways**

*Docker*

Trial 1:
`sudo docker run --name ubvnc -p 6080:80 -p 5900:5900 dorowu/ubuntu-desktop-lxde-vnc:bionic`
`docker start ubvnc`
`docker stop ubvnc`

Trial 2:

`docker run --name ubuntu -it ubuntu`
`sudo apt-get update && sudo apt-get install xinit lxde virtualbox-guest-dkms`
`startx`

*Vagrant*

1. Run the required vagrant file with Team-Viewer installation for now.
2. SSH/RDP into the TeamViewer shell for remote access.
3. Providers provide the shell(TeamViewer) and Consumers SSH/RDP into that shell
4. Solves the NAT problem encountered in docker-networking conatiners.


## Live Demo 
1. Install TeamViewer in your host machine.
2. Provider Server setup in my machine.
3. Login with the following credentials: 
  ```
  id: 
  password:
  ```
  *test user credentials*
  ```
  id: test
  password: password
  ```
4. Connection established.



## TO-DO
1. Improve on security for both providers & consumers.
2. Encrypted access to data.
3. VM Gui needs to be disabled on the provider side.
4. Remove dependency on the TeamViewer Software by building inhouse deployment software.
