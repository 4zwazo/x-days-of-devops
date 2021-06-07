# Jenkins on a raspberry pi 4

### Installing docker

- sudo apt install docker.io

## Create volume

- sudo docker volume create jenkins_home

### Installing Jenkins docker image

- docker run --name jenkins_home \
            --detach \
            -v jenkins_home:/var/jenkins_home \
            -p 8080:8080 \
            -p 50000:50000 \
            nazman/jenkins-armhf

### get initial adming password

- docker exec jenkins_home bash -c cat 'cat /var/jenkins_home/secrets/initialAdminPassword'
- record password

### Initialized Jenkins

- <https://cicd.jeremieonline.com:8080>
- enter password
- choose suggested plugins

-

# Installing nodejs on the container

- login as root
  - docker exec -u 0 -it <containerID> bash
  - apt update
- Installing curl
  - apt install curl
- Install nodejs
  - cd tmp
  - cat /etc/issue
  - curl -sL <http://deb.nodesource.com/setup_14.x> -o nodesource_setup.sh
  - bash nodesource_setup.sh
  - apt install nodejs
- Check version install
  - nodejs -v
  - npm -v

### References

- <https://hub.docker.com/r/nazman/jenkins-armhf>
