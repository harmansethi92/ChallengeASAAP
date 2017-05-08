# ChallengeASAAP

Task 1:
BuildScript
I have created a simple jenkins parallel pipeline to buil;d the servers in integration mode. We can add functionalities such as whenever a new git commit is pushed into repo, continuos build using poll SCM, to build after running a different project first etc

Task2:
To deploy multiple scripts to multiple servers I have created an ansible playbook and host inventory file. In the ansible-playbook you have to install the go Binary depending on your machine. You don't require to install python binary for vagrant machines.
You can just add the server ID to inventory file to which you want to deploy your scripts

Task 3:
I have created a vagrantile to spin up a server and then using command "vagrant provision to run my ansible playbook which is gonna deploy my scripts to multiple servers at once"

Task 4:
To have zero downtime for our servers we could implement Blue-green deployment scenario which acts on the basis of upgrading your application without any downtime to your customers.
