KeePass Access Based Control

Upload your KeePass .kdbx database to kBac Docker container, and access your Passwords/PIN(s)/Secrets from smartphone, PC, tablet.

https://hub.docker.com/r/iblocker/kbac



Installation

```
docker pull iblocker/kbac:v1.0.0

docker run --name containerkbac -d -p 8087:80 iblocker/kbac:v1.0.0
```
Open in browser http://localhost:8087 and login with iblocker/Test#1234

Note: v1.0.X is for amd64, v2.0.X is for arm

![](https://www.2transfer.eu/github/pics/kbac.png)
