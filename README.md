node efficient way to install node js with specific version
==============================================================
> **Note:**
Please avoid to install Node.js with apt-get on Ubuntu. If you already installed Node.js with the built in package manager, 
please remove that. 
```
sudo apt-get purge nodejs && sudo apt-get autoremove && sudo apt-get autoclean

```
STEP1: 
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash

STEP2:
$ nvm list
$ nvm ls-remote
$ nvm install 6.9.4
$ nvm use 6.9.4
$ nvm alias default 6.9.4
$ node -v
$ npm install -g npm
$ npm -v
```
> **Tip:** Check out the > Don’t forget to run the following command, which increases the amount of inotify watches.
```
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```


### inspired from
https://github.com/creationix/nvm
