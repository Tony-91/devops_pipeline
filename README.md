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











