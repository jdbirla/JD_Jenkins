# Learn GitLab CI/CD from a GitLab Hero. Obtain valuable DevOps skills. Build pipelines & Deploy to AWS.
- https://precisely.udemy.com/course/gitlab-ci-pipelines-ci-cd-and-devops-for-beginners/learn/lecture/15108710?start=1#overview
- The alternative is to set up your own GitLab runners, which is a path I don't recommend for beginners.
However, if you wish to do so, here is a very simple tutorial on how to do that:

- Setup GitLab CI Runner with Docker Executor on Windows 10/11 : https://medium.com/devops-with-valentine/setup-gitlab-ci-runner-with-docker-executor-on-windows-10-11-c58dafba9191?sk=b550a70c0a7a60f1a3250a53145a3541
- How to Configure your own GitLab Runner with a Docker Executor on AWS EC2 : https://youtu.be/HGJWMTNeYqI
- How to configure your own Gitlab CI Runner (macOS). : https://www.youtube.com/watch?v=G8ZONHOTAQk

## Introduction 
- https://learn.getgrav.org/16/advanced/yaml
```yml
stages:
    - build
    - test

build:
    stage: build
    script:
        - echo "Building"
        - mkdir build
        - touch build/info.txt
    artifacts:
        paths:
            - build/

test:
    stage: test
    script:
        - echo "Testing"
        - test -f "build/info.txt"
```
- yml : https://learn.getgrav.org/16/advanced/yaml
- SSH git windows : https://www.youtube.com/watch?v=Vmt0V6a3ppE , https://medium.com/devops-with-valentine/2021-how-to-your-ssh-key-for-gitlab-on-windows-10-587579192be0

### GIT Architecture


