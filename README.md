# Kinsta-Git-Deploy
Git hooks that help deploying via git to Kinsta

How to setup git at kinsta so it works like WPEngine: https://anchor.host/automatic-git-deploy-with-kinsta-via-ssh/

post-receive hook is absed on Austin Ginders deploy script and extended with permission checks.

pre-receive is a php syntax checker that makes sure you don't submit problematic code to the repository

thanks to https://kinsta.com and https://twitter.com/austinginder and https://anchor.host/
