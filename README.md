# dockerbox
Super simple Vagrant box to experiment with Docker.

This Vagrant box lets you experiment with Docker in a clean box without having to go through the hassle of installing docker over and over again.

The provision script follows the intallation procedure as documented on https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/.

As post installation steps, the ```vagrant``` user is added to the ```docker``` group so you don't have to put ```sudo``` in front of all your ```docker``` commands. Also, the docker daemon is configured to be started at boot.

Make sure you have Vagrant and Oracle Virtualbox installed on your machine. Then, clone this repository and get started with:

```
vagrant up
vagrant ssh
```

And there you go, you are in your clean version of dockerbox.

Want to see if it all works? Simply run:

```
docker run hello-world
```

Time for a fresh start? No problem. Simply throw away your old dockerbox and create a new one:

```
vagrant destroy
vagrant up
```
