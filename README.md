# 2a_Stop_and_Wait_Protocol
## AIM 
To write a python program to perform stop and wait protocol
## ALGORITHM
1. Start the program.
2. Get the frame size from the user
3. To create the frame based on the user request.
4. To send frames to server from the client side.
5. If your frames reach the server it will send ACK signal to client
6. Stop the Program
## PROGRAM
CLIENT
```
client.send(msg.encode())  

if msg.lower() == 'exit':  
    print("Connection closed by client")
    client.close()
    break

try:
    ack = client.recv(1024).decode()
    if ack == "ACK":
        print(f"Server acknowledged: {ack}")
except socket.timeout:
    print("No ACK received, retransmitting...")
    continue

    client

    import socket

```

SERVER
```

if data:
    print(f"Received: {data}")
    conn.send("ACK".encode())

    if data.lower() == 'exit':  
        print("stop and wait completed")
        conn.close()
        break
````

## OUTPUT

https://github.com/gnanapragathika-jpg/2a_Stop_and_Wait_Protocol/blob/main/Screenshot%202026-03-14%20092013.png

https://github.com/gnanapragathika-jpg/2a_Stop_and_Wait_Protocol/blob/main/Screenshot%202026-03-14%20092033.png

## RESULT
Thus, python program to perform stop and wait protocol was successfully executed.
