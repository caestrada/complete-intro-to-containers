# [Complete Intro To Containers](https://frontendmasters.com/courses/complete-intro-containers/introduction/)

- [X] Introduction
- [X] Containers
- [ ] Docker

Course Website - [LINK](https://btholt.github.io/complete-intro-to-containers/)

## Notes

### Docker Notes
* In **Docker** a pre-made `container` is called and `image`.

#### Commands
```bash
docker ps   # will show you all docker containers running
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