# Squad LCV Labo Technical specifications


##  Technical solution description

The Squad LCV Labo consist in an OVH Server. It is installed with Ubuntu LTS 16.04.
The virtualization solution used is KVM with OVS bridges.

Hardware description :
CPU :  Intel  Xeon E5-1650v3 - 6c/12t - 3,5GHz /3,8GHz
RAM :  128Go DDR4 ECC 2133 MHz


The server have 900GB SSD drives used for operating system and curently running VMS.
We have a backup storage of 2x2To SATA drives. This will be used to stock non-runnning VMs disks and all related configuration files.


### Server Installation

The installation of the server is done using OVH templates on SSD drives.


### Server configuration

Server configuration is performed by an Ansible script using IaaC precept.
All is commited and shared in this github project.

All code will be tested / linted using a Github CI module.

The configuration deployment on server will be done with also a github CI module.
We will so apply CI/CD principles to this infrastructure. All the configuration of 
the server will be performed using this way. We will limit usage of root account on
the server to the minial urgency usages.

### 

