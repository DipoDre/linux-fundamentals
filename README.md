
<!-- ABOUT THE PROJECT -->
## LINUX FUNDAMENTALS

### Objective

For this project, the following steps were taken to demonstrate linux fundamentals:

- [LINUX FUNDAMENTALS](#linux-fundamentals)
  - [Objective](#objective)
    - [Creation of AWS Account](#creation-of-aws-account)
    - [Virtual Server(Instance) Creation](#virtual-serverinstance-creation)
    - [Connecting to the Server](#connecting-to-the-server)
    - [Software Management](#software-management)
      - [Installing A Software](#installing-a-software)
      - [Updating A Software](#updating-a-software)
      - [Removing A Software](#removing-a-software)

----

#### Creation of AWS Account

Register for a new AWS account and sign in.

![Alt text](img/1-aws-account.png)

----

#### Virtual Server(Instance) Creation

Navigate to EC2 home and select Instances.


![Alt text](img/2-ec2-home.png)

On the Instances page click on the Launch Instance button.

![Alt text](img/3-ec2-instance.png)


Fill the required text fields and select options eligible applicable to free tier.
This example uses the Ubuntu distribution of linux. 

![Alt text](img/4-launch-instance.png)

![Alt text](img/5-launch-instance-2.png)

Generate an access key to enable SSH connection.

![Alt text](img/6-launch-instance-3.png)

Afterwards, launch the instance.

Navigate to the instance home page to see the newly created instance
![Alt text](img/7-launched-instance.png)

----

#### Connecting to the Server

Open your terminal.
Run the command chmod 400 "key.pem" to make the key private
Using the ssh command and pem file (key) access the new instance on its ip address.

![Alt text](img/8-connecting-to-server.png)

----


#### Software Management

Software can be installed, updated and removed with the help of a package manager.
Since this is an Ubuntu server, the package manager is apt.

##### Installing A Software

Refresh the package lists by running the command "sudo apt update"


![Alt text](img/9-update-repositories.png)

Install a software by running the command "sudo apt install [software-name]" e.g. "sudo apt install tree"

![Alt text](img/10-install-software.png)


Test the installed software by running the command "tree"

![Alt text](img/11-run-tree-cmd.png)

----

##### Updating A Software

Keep the system up-to-date by running the command "sudo apt upgrade"

![Alt text](img/12-update-packages.png)

----

##### Removing A Software

A software can be removed by running the command "sudo apt remove [software-name]" e.g. "sudo apt remove tree"

![Alt text](img/13-uninstall-software.png)



