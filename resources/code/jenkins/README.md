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

### References

- <https://hub.docker.com/r/mlucken/jenkins-arm>
- <https://hub.docker.com/r/nazman/jenkins-armhf>
- <https://www.gdcorner.com/2019/12/27/JenkinsHomeLab-P1-MasterSetup.html>
