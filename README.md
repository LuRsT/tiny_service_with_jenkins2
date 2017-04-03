# I am tiny

A tiny python app that is built using Jenkins with a `Jenkinsfile` as a pipeline

This is the smallest example I found to learn about `Jenkinsfile`s

## How to use:

    docker pull jenkins
    mkdir /tmp/jenkins
    docker run -p 8080:8080 -p 50000:50000 -v /tmp/jenkins:/var/jenkins_home jenkins

Point your browser to http://localhost:8080. Jenkins will ask for a password,
open a new terminal and do this:

    cat ~/secrets/initialAdminPassword

Copy paste the result into your browser and proceed with the setup wizard.

Next you want to setup a new project using "Pipeline", there's an option at the
bottom to get the `Jenkinsfile` from an SCM, pick this repo and press "Build
now".

Done!
