## Install Ubuntu in Virtual box

In our first gatherin, we set-up the environment. From scratch, we installed Ubuntu 18.04 LTS on VirtualBox and install Docker on it and ran ELK stack on Docker. We went a step further to run metricbeat and saw the system data in Kibana Discover, next thing would be setting up metricbeat dashboards. But we are done for now...

### Download virtual box

https://www.virtualbox.org/wiki/Downloads

### Download Ubuntu Desktop

https://www.ubuntu.com/download/desktop

#### Troubleshooting

If the VirtualBox doesn't give you 64-bit options to install Ubuntu:
https://superuser.com/questions/866962/why-does-virtualbox-only-have-32-bit-option-no-64-bit-option-on-windows-7

### Using the terminal (bash, shell, console, scripting)

https://help.ubuntu.com/community/UsingTheTerminal

### Getting git, cloning a git repo

https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

### Install docker

https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce

### Spin up elk server

docker pull sebp/elk
Read the documentation for port forwarding and 
https://elk-docker.readthedocs.io/

### Troubleshooting

vm.max_map_count [65530] likely too low, increase to at least [262144]:
https://github.com/docker-library/elasticsearch/issues/111

```
sudo sysctl -w vm.max_map_count=262144
```

## Where to go from here

- Deep dive into Docker?
  Docker docs for all...
  https://docs.docker.com/
- Oh, dude! Where is my python on Ubuntu!?!
  Easy piecy...
  https://docs.anaconda.com/anaconda/install/linux
- I want nice figures on Kibana!
  Start from sample metricbeat dashboards, metricbeat was on your system anyways...
  https://www.elastic.co/guide/en/beats/metricbeat/5.5/metricbeat-sample-dashboards.html
