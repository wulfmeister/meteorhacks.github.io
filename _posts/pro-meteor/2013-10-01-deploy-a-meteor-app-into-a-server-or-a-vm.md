---
layout: pro-meteor-post
title: Deploy a Meteor App into a Server or a VM
category: prometeor
summery: "In this section, I'll show you how to deploy your Meteor application into a server from AWS Ec2, Digital Ocean or from any other cloud provider."
---

In this section, I'll show you how to deploy your Meteor application into a server from AWS Ec2, Digital Ocean or from any other cloud provider.

## The Easiest Way

There are few command line tools, which allows you to deploy to a server very easily. See following tools.

* [meteor.sh](https://github.com/netmute/meteor.sh)
* [meteor-deployer](https://github.com/xenolf/meteor-deploy)

Both these tools very easy to use and with few simple commands you can deploy and setup your Meteor app into your server.

## The Correct Way

Although above tools deploy Meteor very easily. They are not perfect. If you are looking for a production quality Meteor deployment setup, you should look for following requirements.

* Automatically restart if crashed (use forever)
* Step Down Prividelges
* Daemonize the app and configure to start when server restarted (use upstart, config file)
* Monitor app freezes and restart if needed 
* Easy way to manage configuration with Environmental Variables and settings.json
* Log Management (use winston)
* CPU, Memory and other system metrics tracking (use node-usage or NodeJS os module)
* Support for Binary NPM modules (try git based deployments)
* Git Based Deployment 

There is a huge list of task and if you are trying to do it yourself, I've added links which helps you to get it setup.

> We can help you on this with our **Managed Meteor Deployment** service. Talk to us.