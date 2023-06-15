# vagrant_getting_started

https://developer.hashicorp.com/vagrant/tutorials/getting-started/getting-started-project-setup

```
winget install Oracle.VirtualBox
winget install Hashicorp.Vagrant
```

```
mkdir vagrant_getting_started
cd vagrant_getting_started
vagrant init hach​​icorp/bionic64
```

Vagrantfile
```
Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/bionic64"
end
```

```
vagrant up
vagrant ssh
```

sshから抜ける
```
vagrant@vagrant:~$ logout
Connection to 127.0.0.1 closed.
```

```
vagrant destroy
```

```
vagrant box list
```

```
vagrant box remove hashicorp/bionic64
```