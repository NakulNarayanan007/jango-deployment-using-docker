1.Clone the project to the local.
2.Make sure you install Docker in the system
*) Get the latest Docker package
       curl -fsSL https://get.docker.com/ | sh
	sudo apt-get install docker docker-engine

*) Add yourself to the docker group, log out, and then log back in to ensure that you can run Docker commands without sudo:
 	 sudo usermod -a -G docker $USER

*) Verify docker is installed correctly
	sudo docker run hello-world

3.Move to the project folder path
4.To build Docker image for the  project, Run the following command
    'sudo docker build -t [image_name] .'
eg: sudo docker build -t django_image.

5.Run a docker container with this image, By running this the app will be live.
   ' sudo docker run -d --name [container_name] -i [image_name]'
eg:sudo docker run -d --name Django -i django_image

6.If you check the running Docker containers by using 
'sudo docker ps '.

 in here we can see our container running
7.To check it in our browser, find IP of Docker container build.
'sudo docker inspect [container_name]'

8.Go to that IP in our browser their you can see our app live
