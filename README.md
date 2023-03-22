
Create a folder named docker
open the folder with vs code
create a file name it app.js
console.log("This is docker app");
run the file in the terminal by writing  node app.js
Create Dockerfile file with D capital. (The file has no extension)
Install docker extension in VScode, you may see the recommendation on vs code.
Write into Dockerfile
FROM node:alpine
COPY . /app
WORKDIR /app
CMD node app.js
	Alpine is the Linux extension. 
	Copy everything to the app directory.
	Check app is the current working directory.
	Execute the app.js file with node.
 Run the command to create a tag.
 
Check for the image.
 
The image that we have created contains alpine-Linux, node and application files.
Now run the image that we have just created, -- here we have image named docker.
  
It returns the output from the image.
Now login to the Docker Account
 
Also, login to hub.docker.com and create a repository. 
 

Now change the image name to the new image name as it shows with your account name and repository name, both images would have same image id.
(I was having issue with pulling the container, so I rename the image with the repository)  
 
Push the image to the docker.
 
Now go to the docker playground and login with the credentials 
Add a new instance. 	
 

Pull the image from the docker and check whether it is loaded or not.
Now run the container and you will see the image is running.
 
The image is loaded and working fine.
