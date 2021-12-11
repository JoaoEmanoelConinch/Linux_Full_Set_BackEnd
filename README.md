# Linux_Full_Set_BackEnd
This is a tutorial to you install your  Linux Full Set BackEnd. I'm using an Unbuntu 20.4.

### What will you install in this tutorial?
* JDK / java 11;
* IntelliJ IDEA;

#### JDK / java 11:
1. Update your system using this comands: `you will need to do it all the time you want to install something...`
```
$ sudo apt update upgrade
```
2. To install JDK:
``` 
$ sudo apt install openjdk-11-jdk
```
3. After some time, it will ask you if you want to continue, so you have to press ```y``` to autorizate;
4. And afther it, use the comand ```java --version``` and ```javac --version```;

#### IntelliJ IDEA:
1. Update your systen using this comands:
```
$ sudo apt update upgrade
```
Before you install IntelliJ, you will need to instal `snap`:

`Snap`, or `Snappy` is a technology udes to install desktop apps in Linux.

So, now let's start, you will need to add a `Snapd` repository:
```
echo -e '[gentoo-snappy]\n location = /usr/local/portage/gentoo-snappy\n sync-type = git\n sync-uri = https://github.com/zyga/gentoo-snappy.git\n priority = 50\n auto-sync = yes
\n Categories=Application' | sudo tee /etc/portage/repos.conf/gentoo-snappy.conf
```
