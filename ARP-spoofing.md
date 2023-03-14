# Man in the middle atack (ARP spoofing) - Questions && Answers

### 1. What is the *Address Resolution Protocol (ARP)*, and what is its role in a network?

- The Address Resolution Protocol is a communication protocol used for discovering the phisycal address from the known network address inside the local network.

### 2. What is a Man-in-the-Middle (MitM) attack, and how does ARP spoofing enable it?

- A Man-in-the-Middle attack is a cyberattack where the attacker intercepts messages between two parties and obtains the MAC address from one side. ARP spoofing is a technique by which an attacker sends (spoofed) ARP messages onto a local area network. 

### 3. How does an attacker use ARP spoofing to intercept network traffic?

- The aim is to associate the attacker's MAC address with the IP address of another host causing any traffic meant for that IP address to be sent to the attacker instead.

### 4. How is the cookie used to derive the encryption/decryption key?

- The encryption/decryption key is derived from a cookie using a decryption algorithm

### 5. What REST API request do you need to send to the crypto oracle the secret cookie?

- We need to send the GET /arp/cookie request to the crypto oracle server

### 6. How do you obtain the authentication token?

- The authentification token is obtained via sending the POST request with the arguments: username=${username}; password={password}; /arp/token to the crypto oracle server

### 7. How do you use the authentication token to obtain the cookie?

- Via token authorization to succesfully send the GET /arp/cookie request

### 8. What encryption mode is used to encrypt the challenge in this lab?

- CBC encryption mode

### 9. What tool can you use to capture network traffic on a local network interface?

- tcpdump
