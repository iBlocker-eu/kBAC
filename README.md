KeePass Based Access

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

After user uploads his .kdbx file, the database ID is generated - e.g. acceda388dfc.

In case user wants to change the ID to a friendly name, he has to login to container and change it as below:
```
docker exec -it containerkbac sh
cd /var/www/localhost/cgi-bin/keepass/INSERTED/
mv acceda388dfc.kdbx iBlocker.kdbx
```

