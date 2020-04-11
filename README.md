# Private Blockchain Application

Application where you can run a private blockchain on your local machine. Blocks can be added to the blockchain and the blockchain can be validated.
In the blocks one could save stars.

This application is part of the Udacity blockchain development nano degree.

## What tools or technologies you will use to create this application?

- This application is created using Node.js and the Javascript programming language. 
- The libraries or npm modules used are:
    - "bitcoinjs-lib": "^4.0.3",
    - "bitcoinjs-message": "^2.0.0",
    - "body-parser": "^1.18.3",
    - "crypto-js": "^3.1.9-1",
    - "express": "^4.16.4",
    - "hex2ascii": "0.0.3",
    - "morgan": "^1.9.1"

## Set up/instructions

-Clone/download this repository 

-Run `npm install` in the project directory, this installs all dependencies 

-Run your application using the command `node app.js`
You should see in your terminal a message indicating that the server is listening in port 8000:
> Server Listening for port: 8000

## Tests

The application was tested using POSTMAN, this tool will help you to make the requests to the API.

1. To make sure your application is working fine and it creates the Genesis Block you can use POSTMAN to request the Genesis block:
    ![Request: http://localhost:8000/block/0 ](https://raw.githubusercontent.com/rmotmans/Private-Blockchain-Project/master/screenshots/genesisBlock.png)
    
2. Make your first request of ownership sending your wallet address:
    ![Request: http://localhost:8000/requestValidation ](https://raw.githubusercontent.com/rmotmans/Private-Blockchain-Project/master/screenshots/requestValidation.png)
    
3. Sign the message with your Wallet:
    ![Use the Wallet to sign a message](https://raw.githubusercontent.com/rmotmans/Private-Blockchain-Project/master/screenshots/SignMessage.png)
    
4. Submit your Star
     ![Request: http://localhost:8000/submitstar](https://raw.githubusercontent.com/rmotmans/Private-Blockchain-Project/master/screenshots/submitStar.png)
     
5. Retrieve Stars owned by me
    ![Request: http://localhost:8000/blocks/<WALLET_ADDRESS>](https://raw.githubusercontent.com/rmotmans/Private-Blockchain-Project/master/screenshots/retrieveStars.png)
