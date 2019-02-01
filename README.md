# Kinsta-Git-Deploy
Git hooks that help deploying a WordPress site via Git to Kinsta.com

## Description
The **post-receive** hook script is based on Austin Ginders Kinsta deploy script and extended with permission checks for the Kinsta environment.

The **pre-receive** hook script is a PHP syntax checker that makes sure you don't commit problematic code to the repository and deploy it to your live website.

## Setup

How to setup Git at Kinsta.com so it works similar to WPEngine: https://anchor.host/automatic-git-deploy-with-kinsta-via-ssh/

After following the guide add the **post-receive** and **pre-receive** files to the `/www/sitename_123/private/sitename.git/hooks/` directory at Kinsta. Make sure to make them executable. For the lazy, this also works:

```
cd /www/sitename_123/private/sitename.git/hooks/
wget https://raw.githubusercontent.com/kLOsk/Kinsta-Git-Deploy/master/post-receive
wget https://raw.githubusercontent.com/kLOsk/Kinsta-Git-Deploy/master/pre-receive
chmod +x post-receive
chmod +x pre-receive
```

### IMPORTANT
Make sure to edit the **post-receive** file and adjust `TARGET` and `GIT_DIR` to match your Kinsta environment.

# :neckbeard:

Thanks to https://twitter.com/austinginder, https://anchor.host/ and https://kinsta.com Support :fist:
