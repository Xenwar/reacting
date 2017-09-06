# There are four alternatives to run this app.
  - Using Online deployed version. 
  - Running locally as is
  - Pulling a docker image from dockerhub
  - Building a docker image locally. 
  
## Deployed Version
https://reacting-signup.herokuapp.com/

## Development version

From the root of the application run `npm install && npm start` and 
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

## To run as a docker container, Use one of the following options.

### Options (a), download from docker hub
docker run --name signupapp -p 3000:3000 -d bottledjinni/reactsignup

### Options (b), build it locally. 
#### Use the following commands. 

```
To build the image, run: 
  make build
To run the app, run: 
  make run

You might need to wait for a while until the app comes online. 

open your browser on 
```
http://localhost:3000/
```
To stop the application, run: 
   make stop
To remove the container, run: 
   make remove

To remove the iamge with its dependencies, run: 
   make clean


Note:
If port 3000 is taken, update the Makefile
Either change the port on the left of ':' shown below. 
Or 
kill the processes using the port. 
   To get the pids, run [lsof -i :3000]
 
#change the port in the Makefile, run block 
#docker run -p 3000:3000 -d ${USER}/${DOCKER_IMAGE_NAME}
```



## Summary (done)
- Done, 20 random participants
- Done, Table that displays the participants.
- Done, A form to add new row (very basic non-real life validation.)
- Done, Deletion of a row
- Done, Sorting each column 
- Done, Deployed online
- Not done, inline editing
- Paritally done, UI design
