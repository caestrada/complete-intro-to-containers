# [Complete Intro To Containers](https://frontendmasters.com/courses/complete-intro-containers/introduction/)

- [X] Introduction
- [X] Containers
- [X] Docker
- [ ] The Dockerfile

Course Website - [LINK](https://btholt.github.io/complete-intro-to-containers/)

## Notes

### Docker Notes
* In **Docker** a pre-made `container` is called and `image`.

#### Docker CLI
```bash
docker ps   # will show you all docker containers running
```
```bash
# Docker images could take a lot of space in your computer. To clear some of those run:
docker image prune
```

```bash
# To see all the images
docker image list
```

```bash
# Build a container with the name you specify
docker build --tag my-name-app .
```

```bash
# Here is how I run a node app from Docker
# Notice the ports. 3000:3000
# 8000 is the port I want to export the app in for myself.
# 3000 is the port Im using in my node app.
docker run --publish 8000:3000  my-node-app
```

### Other Notes
In containers you might not know which distribution you are in running the following command is a trick to know:
```bash
$ cat /etc/issue
```

If you want to see the dependent libraries of an executable run:
```bash
# Run the 'ldd' comand on an executable
# ex: on ls
$ ldd /bin/ls
```