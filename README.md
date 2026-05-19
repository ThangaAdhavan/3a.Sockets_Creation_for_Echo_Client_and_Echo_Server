# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in server .
4. Send and receive the message using the send function in socket.
## PROGRAM
```
SERVER:

import socket
s=socket.socket()
s.bind(('localhost',8014))
s.listen(5)
c,addr=s.accept()
while True:
 ClientMessage=c.recv(1024).decode()
 c.send(ClientMessage.encode())

CLIENT:
import socket
s=socket.socket()
s.connect(('localhost',8014))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())
```
## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3a59573e-1271-4ce9-b0fe-9e6b70fa47d2" />
## RESULT

Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
