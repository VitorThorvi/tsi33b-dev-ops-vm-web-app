##  Video 01 - [DevOps1|DevOps2|Cloud] - Virtualizando com Multipass 

* create 3 VM's

Video uses multipass. As I will be using proxmox, will create those 3 VM's by cloning a template that I already have.

config: each VM will have 1GB RAM, 12GB boot disk and 2 vCPUs.

Command: `brctl show` shows taps, connected to virtual bridges.

Command: `ip route` shows gateways

___

## 02 - [DevOps1|DevOps2|Cloud] - Aprendendo Redes Virtuais I 

New definitions: 
    
    SDN : Software defined network
    IaC : Infrastructure as code -> yaml code 

### topics

* hybrid model
* 3 VM's scenario
* switching / bridge
* routing
* NTP
* DNS
* HTTP
* NAT

## Hybrid model 
Joins OSI (reference model) and TCP/IP model to a 5 layer hybrid model.
    
    OSI's 7 layers      ->      Hybrid model
        l7: application                 -> l5 ~ l7 : "l7" : application
        l6: presenttion (html,compression,etc)
        l5: session (sync)
        l4: transport (reliability)     -> l4 : l4 : transport
        l3: network (routing)           -> l3 : network
        l2: data link (NIC protocols. 802.11(wifi); 802.3(ethernet) How physical media receives information)  -> l2 : l2 : data link. 
        l1: physical                    -> l1 : l1 : physical
 

resolvconf application is installed on ubuntu to add to resolv.conf file HEAD current multipass local dns. It enables the local host to interact with VM's by their names. 

resolvconf application is needed because resolv.conf file should not be directly edited.

My installation of multipass has the 10.168.42.0/24 IP range. When multipass is installed, it changes. So the correct ip range must be considered.

``` bash
# edit head to apply desired configuration to the head of resolv.conf file
sudo nano /etc/resolvconf/resolv.conf.d/head

# add nameserver using multipass ip
nameserver 10.168.34.1
```

___


## 03 - [DevOps1|DevOps2|Cloud] - Virtualizando Aplicação Web I

This video will show the implementation of tutorial republic's PHP MySQL CRUD application.

Also, in the end it is expected to implement tcpdump/wireshark to see how the application communicates between VM's

We will have 4 VM's.

As of now, I've standarized a 4 VM's setup. All of them have my text editor of choice (micro), terminal of choice (kitty + zshell). 
Also all of them have build-essential package installed via apt and homebrew for linux installed. 

It is the same script I run for my template VM on proxmox. 

All those 4 VM's have been snapshotted (snap1) and can be restored to the initial state.

Similarly, the class proposes to use 4 VM's. Below are the proposed VM's mapped to my setup

* dev -> vm1
* db -> vm2
* web -> vm3
* DNS -> vm4

> Tutorial republic says the code can't be distributed online, so this repo won't have its code. The code will be stored locally at the VM's


### objetivos

* install mysql
* verify it is reacheable via network
* create a database
* create 'employees' table inside the created db

- [x] all done!


> site useful to understant what a command do: explainshell.com




### now working on vm3 (web)

we'will work with `nginx` web server.


























