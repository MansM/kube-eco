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

# urls after running:
- http://dashboard.example.com
- http://jenkins.example.com
- http://gitlab.example.com
- http://prometheus.example.com
- http://alerts.example.com

(it is really example.com, I need to make it configurable though)

## Todo:
- On Jenkins start build the a new jenkins slave image, containing klar and maybe other binaries
- coreos/clair
- migrate to official gitlab helm charts
- spotify gc
- BELK/EFK
- LDAP
- keycloak or dex (maybeish)
- calico/canal when this can actually work in minikube
