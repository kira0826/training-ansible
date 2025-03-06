# training-ansible

**Kevin Steven Nieto Curaca**

First, pipx is installed to proceed with the installation of Ansible. This allows Ansible to be installed regardless of whether the system is Fedora or another Linux distribution.

![image](https://github.com/user-attachments/assets/388055f3-99c0-4f24-aa8e-624f63068d9d)


Before running the commands, it is necessary to configure the host so that the machine where the container will run is registered, as shown below:

![image](https://github.com/user-attachments/assets/5554d02a-910b-44bd-a488-624e9a573bc4)

The next commands are use to run the pipelines created for ansible to execute some tasks, such  as docker installation and execute the docker container to play mario bros.
First Ansible command:

![image](https://github.com/user-attachments/assets/c3932609-c386-47b1-bebe-808688d381fb)


Second Ansible command:

![image](https://github.com/user-attachments/assets/6a56f03a-fe5b-4da4-82df-2d06e181eb85)


With the above commands, we provision everything necessary on the server so that it can run the Mario game.

To verify that the Mario service is running, we navigate to the IP address and the port set in the main task. It is crucial to activate the security rule to allow traffic through port 8787 both in the NSG and internally on the machine's firewall.

Security rules:
In the NSG:

![image](https://github.com/user-attachments/assets/74e3ba0a-5212-4bfe-9438-80024eb8afde)

In the machine's firewall:


![image](https://github.com/user-attachments/assets/6a8c3a6e-857c-4968-bd08-bab9fc8aa301)

![image](https://github.com/user-attachments/assets/a80cefed-d4ff-42f9-81b4-1afbd740d08c)


Note: Ansible integrates the chosen image or disk. Initially, I had a RHEL image, but I had to change it because many dependencies were focused on Ubuntu, and the Python version was insufficient to run Ansible. Therefore, I migrated to a VM with the following OS configuration:

![image](https://github.com/user-attachments/assets/cf26c97a-5ddd-4b7c-adda-2b59a19acac5)





