## Vagrant
Setup VirtualBox and host sample web server using Vagrantfile

Want to try this:
 Clone this repository:

    
        git clone https://github.com/abhi-kr07/Setup-apche2-using-Vagrant.git
     

Change the host_ip to your localhost ip in Vagrantfile:
      ```
         host_ip: "<your localhost ip>"
      ```

Run the command 
    ```
        vagrant up
    ```

Now, acess your webserver using your localhost IP:
    ```
        <IP:8080>
    ```

## prerequisites
- You need to have *Vagrant* installed in your system: Install it from official website : (https://developer.hashicorp.com/vagrant/install)
- you need to have *VirtualBox* installed in your system: Install it from official website : (https://www.virtualbox.org/wiki/Downloads)
