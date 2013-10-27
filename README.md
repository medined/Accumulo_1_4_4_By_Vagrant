Accumulo v1.4.4 By_Vagrant
=======================

A three node Accumulo cluster running on Ubuntu Precise (12.04). The instance name is 'instance'. The 
user name is 'root' and the password is 'secret'.

1. Install Vagrant
2. Download this project.
3. Add the following to your /etc/host file.

```
10.211.55.100	affy-master
10.211.55.101	affy-slave1
10.211.55.102	affy-slave2
```

4. Run 'Vagrant up'

5. Run 'post_spinup.sh'

Now you can visit the following URLs in your browser:

```
http://affy-master:50095
http://affy-master:50070/dfshealth.jsp
http://affy-master:50030/jobtracker.jsp
```

You can SSH to the nodes using the following commands. Notice that the hostnames start with 'affy-' but that 
the vagrant nodes do not have the prefix.

```
vagrant ssh master
vagrant ssh slave1
vagrant ssh slave2
```
