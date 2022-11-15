# CHAT-APPLICATION-WITH-HYBRID-CRYPTOGRAPHY-TECHNIQUES

DESCRIPTION:

Java's implementation of the generation of public and private RSA keys for a client and a server. 
Messages encrypted with RSA are traded back and forth between a client and a server. AES key generation on the server side, 
followed by RSA-encrypted transmission of the generated key to the client browser. message pass-back and forwarding using AES between a client and a server.

MODULES:

1.RSA MODULE

2.SERVER MODULE

3.CLIENT MODULE

MODULE 1: RSA 

The generated RSA key pair (consisting of a private and public key) will be stored in the specified local files.
This will invoke the create RSA function on a new RSA object.
Keys and specifications are saved in files.

MODULE 2: SERVER

The client's request for a connection has been granted by the server.
When the server agrees to the connection, the client will send it an RSA-encrypted AES key. 
The RSA public key will now be used to decrypt the key on the server. 
The client and server will begin exchanging data now. When a client sends a message to the server, the server will get it in an encrypted form.
It can read and decrypt encrypted data. Since this update, the server can also send messages to the client, and those messages will be encrypted using AES.

MODULE3: CLIENT 

When the server approves the connection, the client will generate an AES key and encrypt it using an RSA key. 
The encrypted AES key and the time it took to encrypt it using RSA are both displayed. 
The client then sends the message to the server, where it is encrypted using AES before being printed to the terminal. 
Each message's encrypting time, in nanoseconds, is also displayed for reference. Also, the server's messages are encrypted before being sent to the client.
The RSA key is used to decrypt the encrypted communication.


