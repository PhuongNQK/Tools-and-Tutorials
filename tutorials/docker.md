# Installation
- https://medium.com/@sebagomez/installing-the-docker-client-on-ubuntus-windows-subsystem-for-linux-612b392a44c4
- https://nickjanetakis.com/blog/setting-up-docker-for-windows-and-wsl-to-work-flawlessly
- https://blogs.msdn.microsoft.com/commandline/2017/12/08/cross-post-wsl-interoperability-with-docker/
- [How to set up Docker and Windows Subsystem for Linux: A Love Story.](https://medium.com/free-code-camp/how-to-set-up-docker-and-windows-subsystem-for-linux-a-love-story-35c856968991)
    
# Getting started
- [Get Started, Part 1: Orientation and setup](https://docs.docker.com/get-started/)
- [Installing Docker Toolbox On Windows](https://www.ibm.com/developerworks/community/blogs/jfp/entry/Using_Docker_Machine_On_Windows?lang=en)
- [Command Line Replacement For Windows](https://manski.net/2016/09/command-line-replacement-for-windows/)
- [Quick Tip: Start Docker Toolbox Shell via Batch](https://manski.net/2016/10/docker-toolbox-shell-via-batch/)
- [Naming Docker Containers: 3 Tips for Beginners](https://www.digitalocean.com/community/tutorials/naming-docker-containers-3-tips-for-beginners)
- For Docker Toolbox:
    + By default, **C:\Users** is the shared folder between the host and the default VirtualBox VM created by Docker. 
    + [How to use a directory outside C:\Users with Docker Toolbox/Docker for Windows](http://support.divio.com/en/articles/646695-how-to-use-a-directory-outside-c-users-with-docker-toolbox-docker-for-windows)
    + By default, Docker API is not accessible from the host. You need to edit file **/var/lib/boot2docker/profile** in the VM to disable TLS verify (set it to **no**) (you may also need to adjust the port to anything other than 2376) and DO NOT SET the environment variable named **DOCKER_TLS_VERIFY** (or setting it to an empty string if you can). Then restart the VM and try to access Docker API from the host using something like: **curl -X GET http://192.168.99.100:2375/images/json** (assuming that you adjusted the port to 2375)
- [How to access and secure the Docker Engine API in Docker Swarm for AWS](https://medium.com/faun/how-to-access-and-secure-the-docker-engine-api-in-docker-swarm-for-aws-a5d67db2c417)
- [Enabling and accessing Docker Engine API on a remote docker host on Ubuntu](https://medium.com/@sudarakayasindu/enabling-and-accessing-docker-engine-api-on-a-remote-docker-host-on-ubuntu-16-04-2c15f55f5d39)

# Sharing data between containers and between containers and hosts
- https://www.digitalocean.com/community/tutorials/how-to-share-data-between-docker-containers
- Docker volumes and file system permissions: https://medium.com/@nielssj/docker-volumes-and-file-system-permissions-772c1aee23ca
- See ranjandas's reply: https://forums.docker.com/t/docker-toolbox-host-folder-permissions/3419/10
- https://4sysops.com/archives/introduction-to-docker-bind-mounts-and-volumes

# Dockerize frontend apps
React: https://medium.com/ai2-blog/dockerizing-a-react-application-3563688a2378 \
Angular 4: https://github.com/avatsaev/angular4-docker-example/blob/master/Dockerfile
Angular: https://www.slideshare.net/johnpapa/optimizing-and-deploying-angular
- [Build & deploy React and Angular2 WebApps automatically with Docker](https://medium.com/@lukin0110/build-deploy-react-and-angular2-webapps-automatically-with-docker-8ba81421f759)

# Dockerize webapps
- SpringBoot with embedded Tomcat:
    + https://spring.io/guides/gs/spring-boot-docker/
    + https://dzone.com/articles/spring-boot-embedded-tomcat-example

# Kubernetes
- Intro to Kubernetes: https://www.xoriant.com/blog/cloud-infrastructure/introduction-kubernetes.html
- Introduction to Kubernetes Building Blocks: https://www.xoriant.com/blog/cloud-infrastructure/introduction-kubernetes-building-blocks.html
- Tutorial : Getting Started with Kubernetes on your Windows Laptop with Minikube: https://rominirani.com/tutorial-getting-started-with-kubernetes-on-your-windows-laptop-with-minikube-3269b54a226
- Running your own Docker containers in Minikube for Windows: https://medium.com/@maumribeiro/running-your-own-docker-images-in-minikube-for-windows-ea7383d931f6

# Optimization
- Python image: 
    + https://github.com/jfloff/alpine-python
    + https://blog.realkinetic.com/building-minimal-docker-containers-for-python-applications-37d0272c52f3
- Golang image:
    + https://blog.codeship.com/building-minimal-docker-containers-for-go-applications/
- https://towardsdatascience.com/slimming-down-your-docker-images-275f0ca9337e
- https://medium.com/@gdiener/how-to-build-a-smaller-docker-image-76779e18d48a

# Useful Docker images
- Alpine with envsubst: https://github.com/cirocosta/alpine-envsubst
    + How to use envsubst: https://stackoverflow.com/questions/14155596/how-to-substitute-shell-variables-in-complex-text-files
