FROM python:3.10-slim-buster
#
#Inside the container
#Make a new folder inside the container
WORKDIR /backend-flask

#Outside the Container -> Inside the Container
#This contains the libraries that we want to install to run the app
COPY requirements.txt requirements.txt

#Inside the  Container
#Install the python libraries used for the app 
RUN pip3 install -r requirements.txt

#Outside the  Container -> Inside  the Container
#. means everyting in the current directory
#the first . period means everything in the /backend-flask (ourside container)
#the second . period /backend-flask (inside container)
COPY . .

#env vars configure our app. the below sets them. 
#They are set inside the container and will remain set when the cont is running. 
ENV FLASK_ENV=development
#you can't start up your app without feeding in the env vars. Go to your app and add them



EXPOSE ${PORT}
#Command
#In the [] are the commands that we need to run flask. See, let's type them out:
#python3 -m flask run --host=0.0.0.0 --port=4567
#-m tells system to run mojo in flask
#0.0.0.0 is the EVERYTHING address. It makes the cont run on the qthing host, not your local host
#you can use other ports, but Flask likes this port number. 
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]
#What is the diff between CMD and run?
#CMD---this is a command that the cont will run when it starts up. 
#the CMD actually runs inside the cont image.
#run---a command we are running to create a layer in an image. this is the setup process

#want to check your images? in the terminal, run the command "docker images"


# think of tags -t as different versions you have
# you don't specify a tag? It sets it's own tag for you. Don't use --latest. It's 
#a default tag and that can confuse people! Treat latest as a default. 

#an advantage to contanerization is that it sets things up for us to have them run

#when you have a cont running, you can check the docker logs if you right click on the conts
#ATTACH SHELL FROM THE DOCKER LOGS!!!!!!!!!!! You can run env here and see
#what env vars exist here. 
#-d runs the cont in the background, which is typically what we want to do
#-rm makes the docker clean up. If you don't run it, it exits. You want the Docker cont
# to persist so you can pick up artifacts? --rm makes docker reap the cont and get rid of it.
#