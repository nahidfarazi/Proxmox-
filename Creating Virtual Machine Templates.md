# Creating Virtual Machine Templates
1. #### check ssh host key
```sh
ls -la /ec/ssh
```
2. #### Delete host key
```sh
cd /etc/ssh
```
```sh
sudo rm ssh_host_*
``` 
3. #### install cloud-init
```sh
sudo apt install cloud-init
```
4. #### now empty machine id
```sh
sudo truncate -s 0 /etc/machine-id
```
5. #### machine id node link
```sh
sudo ln -s /etc/machine-id /var/lib/dbus/machine-id
```


   <!--    t         -->
