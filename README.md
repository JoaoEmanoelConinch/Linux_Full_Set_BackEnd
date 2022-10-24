# ⚔️ Linux_Full_Set_BackEnd  <img align="center" height="50" width="50" src="https://img.vivaolinux.com.br/imagens/artigos/comunidade/1427239737.512px-Tux.svg.png"> 

This is a tutorial to you install your  Linux Full Set BackEnd. I'm using an Unbuntu 20.4.

### What will you install in this tutorial?
* [JDK / java;](#jdk)
* [IntelliJ IDEA;](#intellij)
* [PostgreSQL;](#postgres)
* [DBever;](#dbever)
* [Docker;](#docker)

<div alige="center" id='jdk'>

******
    
#### JDK / java 11 or 17:

1. Update your system using this comands: `you will need to do it all the time you want to install something...`
```
$ sudo apt update
```
and
```
$ sudo apt upgrade
```
2. To install JDK:
``` 
$ sudo apt install openjdk-11-jdk
```
or
``` 
$ sudo apt install openjdk-17-jdk
```    
> JDK 17 is the last LTS Java version, but JDK 11 is the most used.
3. After some time, it will ask you if you want to continue, so you have to press ```y``` to autorizate;
4. And afther it, use the comand ```java --version``` and ```javac --version```;

</div>
<div alige="center" id='intellij'>
    
*******

#### IntelliJ IDEA:
>It is an integrated development environment written in Java

1. Update your systen using this comands:
```
$ sudo apt update
```
and
```
$ sudo apt upgrade
```
Now to install the IntelliJ community use this comand:(FREE)
```
$ sudo snap install intellij-idea-community --classic
```
To install the IntelliJ ultimate use this comand:(NOT FREE)
```
$ sudo snap install intellij-idea-ultimate --classic
```
To update IntelliJ use:
```
$ sudo snap refresh intellij-idea-community
```
or
```
$ sudo snap refresh intellij-idea-ultimate
```
Did you see the word `snap`?

`Snap`, or `Snappy` is a technology used to install desktop apps in Linux.
    
 > If you get this error `sudo: snap: command not found`, you can take a look [HERE](https://www.edivaldobrito.com.br/suporte-a-pacotes-snap-no-linux/)

</div> 
<div alige="center" id='postgres'> 
    
****
    
#### PostgeSQL:
> It is a system to manege relational databases

1. Update your systen using this comands again:
```
$ sudo apt update
```
and
```
$ sudo apt upgrade
```
Now you can install postrgres with a pakege `-contrib` to have more funcionalities:
```
$ sudo apt install postgresql postgresql-contrib
```
> Now postgresql created a user `postgres` in your machine, in postegresql we have `roles`, thets how postegreslq calls users.

You can use the comand:
```
$ sudo -i -u postegres
```
to start to use this `user/role`
And to open the pronpt to use `psql` comands use:
```
$ psql
```
Or in you sudo user you can use the comand:
```
$ sudo -u postgres psql
```

</div>
<div alige="center" id='dbever'>
    
****
    
#### Dbever:
> DBeaver is a nice open source alternative to manage Databases

Update your systen again: `$ sudo apt update upgrade`

And now, it's just to rum the comand
```
$ sudo snap install dbeaver-ce
```

</div>
<div alige="center" id='docker'>
    
****  

#### Docker:
> Docker Desktop helps you build, share, and run containers easily on Mac and Windows as you do on Linux.

Update your systen again: `$ sudo apt update upgrade`

Set up the repository
* install packages to allow `apt` to use a repository over HTTPS:
```
$ sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```
* Add Docker’s official GPG key:
```
$  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```    
    
****

</div>
    
### Search Sources
* [Jdk / java11](https://www.linode.com/docs/guides/how-to-install-openjdk-on-ubuntu-20-04/)
* [IntelliJ IDEA](https://www.edivaldobrito.com.br/ide-intellij-idea-no-ubuntu-debian/)
* [snap](https://www.edivaldobrito.com.br/suporte-a-pacotes-snap-no-linux/)
* [PostgreSQL](https://www.digitalocean.com/community/tutorials/how-to-install-postgresql-on-ubuntu-20-04-quickstart-pt)
* [Dbver](https://www.how2shout.com/linux/how-to-install-dbeaver-on-ubuntu-20-04-lts/)
* [Docker](https://docs.docker.com/engine/install/ubuntu/)
