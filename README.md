# Using Vagrant:

vagrant init

atom .

open **'vagrantfile'** and change base to the selected package you want to install.
in this case it will be **'ubuntu/bionic64'**. save it then do next step

Then **'vagrant up'**

Then **'vagrant ssh'**


# How To Update Packages:
sudo apt-get update -y

# How To Install Packages:
sudo apt-get instal <package name> -y

  - In This Case: **'sudo apt-get nginx -y'**

  - Once installed Then Run: **'sudo systemctl start nginx'**

  - Lastly Type: **'ps aux | grep nginx to check it is running'**

# To end the program:
Type 'exit' To Exit Ubuntu.

now go into config file and type:

- **config.vm.network "private_network", ip: '192.168.10.100'**

once thats in save the file and run vagrant reload in terminal

this will reload your vm without destroying it and will update the ip address.

once this is done type in the ip address into the browser and it will give you a welcome page for nginx.
