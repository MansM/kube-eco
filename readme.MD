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


## Todo:
- On Jenkins start build the a new jenkins slave image, containing klar and maybe other binaries
- coreos/clair
- migrate to official gitlab helm charts
- spotify gc
- BELK/EFK
- LDAP
- keycloak or dex (maybeish)
