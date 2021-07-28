# Project Web2

***

### About project

* Application in golang

 * The app displays "Hello, World 2!"

 * You can view it in your browser at http://localhost or http://host_ip

* Dockerfile with information how to builds docker image

* Jenkins pipeline scripts for build and deploy project

***

'''
You can test app, before use it in CI/CD
'''

### Host requirements and preparation:

* Installed Docker

* Installed svn

* Installed curl

***

### Build and deploy

Download project from GitHub

```
svn export https://github.com/Xarakipi/TIL/trunk/exam/project_web2
```

Build docker image

```
sudo docker build -t project_web1 project_web2/
```

Run docker image

```
sudo docker run -d -p 80:80 project_web2
```

Open in your browser http://localhost/
