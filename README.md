# SocketWebAppBot
Server for running Rasa Bot integrated over a webpage through socket channel.

## Prerequisite
- Node JS
- NPM


## Steps:
- step 1: clone this repository

- step 2: go to the project directory

- step 3: edit the [index.html](https://github.com/JiteshGaikwad/SocketWebAppBot/blob/022e8465ba3ad03bff8efb4e266c2476bcc2580f/index.html#L18) add the `socketUrl` value of your Rasa server, instead of writing `localhost` replace it with your ip address where the rasa server is running
 > socketUrl: "http://192.168.0.1:5005"
  
- step 4: Start the Rasa server by running the below command:
>  rasa run -m models --enable-api --cors "*" --debug  
* Make sure you have registered your bot with socket.io channel *

- step 5: Once you have your rasa server running, run the below commands in the project directory:
```
npm install 

npm start
```
*the above commands will install the required dependencies ans start the server*
- step 4: Once you had successfully executed the above command, open your browser with the below url:

> http://localhost:3000/

you will see the webchat in the browser

if you want to run the bot on a system  other than your local sysem, you can open it by replacing the `localhost` with your local system's ip address, for e.g., refer the below url:
> http://192.168.0.1:3000/

**Note**: *if you are accessing from other system, make sure both the local system and other system are connected within the same network*
