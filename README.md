![]()

# FULL DevOps pipeline project | CI/CD | Jenkins | Ansible | Kubernetes 

### Learning Objectives:
1. DevOps
2. Continuous Integration
3. Continuous Delivery

### Technologies and Protocols:
* Jenkins 
* Ansible
* Kubernetes
* Docker

### What the heck is DevOps?
- A consistent streamline and manageable pipeline for software development and delivery 
- Continuous integration and continuous development and continuous testing
- Development and operational teams working cohesively - no more silos!

## Overview:
There are two main parts to this project:
1. Continuous Integration (CI): the practice of merging all developers' working copies to a shared mainline several times a day. Every revision that is committed triggers an automated build and test.
* Step-by-step overview of CI:
    - We update source code on local workstation > we commit the code onto Github repository > Jenkins pulls the code and, with the help of Maven, builds WAR file (build artifacts); Jenkins *pushes* WAR file onto Ansible > Ansible-playbook creates image from WAR file and *commits* it onto docker hub 

2. Continuous Delivery (CD): software engineering approach in which teams produce software in short cycles, ensuring that the software can be reliably released at any time. A practice that uses automation to speed the release of new code.
* Step-by-step overview of CD:
    - After Jenkins NEW image build is successful we can trigger a CD job > Ansile-playbook uses updated image and *pushes* it onto a Kubernetes cluster for end-user access.

> What we are trying to accomplish with DevOps is how can we EFFICIENTLY, EFFORTLESSLY and AUTOMATICALLY update new software to end-users.
 
![]()

### Continuous Integration (CI)
![](images/OVERVIEW.png)

We can edit and commit new changes on GitHub > after, we can run it through Jenkins (“Build Now” to create and push new artifacts - *we can automate this as well!*) and see live updates on the Tomcat server - Maven helps with error checks and simplifying source code. Jenkins and Maven work together to create a SOLID source code foundation to work on. #git2server

A lot of the steps involved setting up and configuring each piece of the environment (software engineer / software architect), also creating admin users and key pairs. I needed to download and configure plugins; plus, I needed to configure variables on the servers to make my life easier (a lot of administrative tasks).But after the initial setup, up I see how streamlines this automatic integration can be absolutely crucial in software development.  Even if the pieces of software to run checks and deploy the code is different, the end goals remains the same: find and address bugs quicker, improve software quality AND reduce the time it takes to validate and release new updates.











