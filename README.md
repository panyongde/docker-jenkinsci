#Jenkins Docker 
[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://paypal.me/nilportugues)

Contains:

- Jenkins
- Java 8
- PHP7
- NodeJS
- NPM
- SQLite
- Ansible
- Ansistrano

## Jenkins Plugins

The following plugins come installed by default: 

```
postbuild-task:1.8
postbuildscript:0.17
jobgenerator:1.22
disable-failed-job:1.15
greenballs:1.15
s3:0.8
docker-plugin:0.16.0
diskcheck:0.26
timestamper:1.7.4
build-pipeline-plugin:1.4.9
naginator:1.16.1
git:2.4.2
ansicolor:0.4.2
build-monitor-plugin:1.8+build.201601112328
build-timeout:1.16
rebuild:1.25
heavy-job:1.1
cucumber-testresult-plugin:0.8.2
ssh-agent:1.9
role-strategy:2.2.0
git-changelog:1.7
```


## Jenkins SSH Key `id_rsa.pub`


Output the contents by issuing: 

```
docker run -it dockerjenkins_jenkins bash -c "cat /home/jenkins/.ssh/id_rsa.pub" 
```
This has to be done from your machine. 

## Password-less SSH for remote machines

For each machine, you'll have to pass your public id_rsa.pub. This should be done with a command that should be along the lines of:

```
docker run -it dockerjenkins_jenkins bash -c  "cat ./home/jenkins/.ssh/id_rsa.pub | ssh user@host -p22 'cat >> ./.ssh/authorized_keys'"
```



# Contribute

Contributions to the package are always welcome!

* Report any bugs or issues you find on the [issue tracker](https://github.com/nilportugues/docker-jenkins/issues/new).
* You can grab the source code at the package's [Git repository](https://github.com/nilportugues/docker-jenkins).


# Support

Get in touch with me using one of the following means:

 - Emailing me at <contact@nilportugues.com>
 - Opening an [Issue](https://github.com/nilportugues/docker-jenkins/issues/new)


# Authors

* [Nil Portugués Calderó](http://nilportugues.com)
* [The Community Contributors](https://github.com/nilportugues/docker-jenkins/graphs/contributors)
