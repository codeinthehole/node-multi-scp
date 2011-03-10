node-multi-scp
==============

This is a simple utility script that allows a file to be copied to all the 
hosts defined in `~/.ssh/config`.

It is assumed that you have copied your public key to each host within `~/.ssh/config`
so the copy can take place without a password prompt.

Note that the [`optimise` module](https://github.com/substack/node-optimist) is a requirement. 

Example usage:

    ./multi-scp ~/.bashrc              # copy ~/.bashrc to all hosts
	./multi-scp sample.bashrc .bashrc  # copy sample.bashrc to all hosts but with remote name .bashrc

node.js is used within the function to spawn a separate child process for each copy.