# node-ubuntu-automate
Quickly deploy an example production ready node application on Ubuntu.
Will work on fresh install of ubuntu (14.04 / 16.04 tested)

What does it do?

#1) Install the VM's required dependencies (Node, Git)

#2) Adds a 1gb swap partition (The VM I use comes with 20gb of SSD but only 512mb ram, This will give us some more room to play with **)

#3) Install nginx to forward any traffic on port 80 over to our node server (Sitting on port 8080 by default).

#4) Clone a node application and then start this as a background service (We use PM2 in this case)

Usage

- Clone this repositery into any folder on your new digitalocean VM (Or just copy the script + default file over)

- run "sudo ubuntu_node_automate.sh" to fire off the script


** This is tested on DigitalOcean $5/month VM. If you're looking to sign up this link will give us both a few months free  https://m.do.co/c/1b0abae63ce7.
