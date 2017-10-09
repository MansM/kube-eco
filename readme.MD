# my kubernetes eco system local demo

## Requirements:
- macOS
- brew ( https://brew.sh/ )
- ansible (brew install ansible )
- minikube ( brew cask install minikube )
- kubectl ( brew install kubernetes-cli )
- dnsmasq ( brew install dnsmasq )
- in your sudoers file: username ALL=NOPASSWD: /usr/local/bin/brew services restart dnsmasq
- probably more... when you find it, please create an issue
- RAM, lots of it ;-) (default setting is now 8192MB for the VM)

## How to run
```
ansible-playbook setup.yaml
```
coffee! it takes a while (especially on slow internet connections)
on my 2015 mbp with 150MBit it takes about 10 minutes

to clean it up: minikube delete

## urls after running:
- http://dashboard.example.com
- http://jenkins.example.com
- http://gitlab.example.com
- http://prometheus.example.com
- http://alerts.example.com

( it is really example.com, you can change it in inventory/group_vars/all.yaml )

## Todo:
- On Jenkins start build the a new jenkins slave image, containing klar and maybe other binaries
- coreos/clair
- migrate to official gitlab helm charts
- spotify gc
- BELK/EFK
- LDAP
- keycloak or dex (maybeish)
- calico/canal when this can actually work in minikube
