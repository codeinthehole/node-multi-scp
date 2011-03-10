node-multi-scp
==============

This is a simple utility script that allows a file to be copied to all the 
hosts defined in `~/.ssh/config`.

It is assumed that you have copied your public key to each host within `~/.ssh/config`
so the copy can take place without a password prompt.

Note that the (`optimise` module)[https://github.com/substack/node-optimist] is a requirement. 