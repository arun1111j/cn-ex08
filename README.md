# EX-8 APPLICATION USING TCP SOCKETS - CREATING ECHO CLIENT-SERVER
# APPLICATION USING TCP SOCKETS - CREATING ECHO CLIENT-SERVER



# EXP: 8

# DATE:26-04-2023

# AIM:
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.

# ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
server.
4. Send and receive the message using the send function in socket.
# PROGRAM:
# CLIENT:
```python3
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
   msg=input("Client > ")
   s.send(msg.encode())
   print("Server > ",s.recv(1024).decode())
  ```
# SERVER:
```python3
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
   ClientMessage=c.recv(1024).decode()
   c.send(ClientMessage.encode())
```

# CLIENT OUTPUT : 
![image](https://github.com/arun1111j/cn-ex08/assets/128461833/193b2a05-2489-46a0-b8ab-6acc2c2fa637)


# SERVER OUTPUT :
![image](https://github.com/arun1111j/cn-ex08/assets/128461833/08d9a76b-5f1d-49a7-a8c6-87b77e34ee7a)



# RESULT:
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links
was successfully created and executed.

DATE :

AIM :


ALGORITHM :


PROGRAM :


OUTPUT :



RESULT :
