# public-config


## commands to get the files
Files will be copied to the default location for the current user.

### Generic aliasses for inside e.g. .bashrc
```
alias verbind='tmux a || windows'
alias dirx="du --si --max-depth=1"
alias mediax="df --si |grep 'media\|Filesystem'| (sed -u 1q; sort -k 6)"
alias dockerips="docker inspect -f '{{.Name}} - {{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' $(docker ps -aq)"
```

### Generating a new key pair
```
ssh-keygen -t rsa -b 4096 -C "<youremail@example.com>"
```


### docker config.json - ~/.docker/config.json
```
wget -q -O - https://raw.githubusercontent.com/phixels/public-config/main/.docker/config.json | sudo tee ~/.docker/config.json
```

### tmux .tmux.conf - ~/.tmux.conf
```
wget -q -O - https://raw.githubusercontent.com/phixels/public-config/main/tmux/.tmux.conf | sudo tee ~/.tmux.conf
```
