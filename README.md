# Useful-Elastic-Beanstalk-Extensions
This is a collection of working, useful ElasticBeanstalk Extensions

## 00_blockdevice-xvdcz.config
Attach a blockdevice volume of 100GB to the EC2 instances created by Beanstalk


## 01

## 02

## 03_docker_thinpool_cleanup.config
This extension is also primarily used for Jenkins in docker. There's an issue with how the thinpools memory is released 
in docker. The issue is that it basically doesn't release used memory without being told to. 
This constantly hits it every half hour and has it release the memory

## 04_docker_cron_cleanup.config
This extension is primarily used for Jenkins in docker to clean up the constant builds being done and taking up space in the thinpool.
It uses an environment variable to set up a regex for how often the cron should run.
