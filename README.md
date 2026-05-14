# public-config


## commands to get the files
Files will be copied to the default location for the current user.

### docker config.json - ~/.docker/config.json
```
wget -q -O - https://raw.githubusercontent.com/phixels/public-config/main/.docker/config.json | sudo tee ~/.docker/config.json
```

### tmux .tmux.conf - ~/.tmux.conf
```
wget -q -O - https://raw.githubusercontent.com/phixels/public-config/main/tmux/.tmux.conf | sudo tee ~/.tmux.conf
```
