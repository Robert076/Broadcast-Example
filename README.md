 Write an UDP broadcast application that serves as client and server at the same time. The application is started with the network broadcast address (<NBCAST>) as argument in the command line.

1.    Upon launching the application listens on UDP port 7777.
2.    Every 3 seconds the application sends a UDP broadcast message to NBCAST port 7777 with the format: TIMEQUERY\0 (string)
3.    Whenever the application receives a TIMEQUERY demand it answers to the source IP:port with a string message: TIME HH:MM:SS\0 (current time) using unicast.
4.    Every 10 seconds the application sends a UDP broadcast message to NBCAST port 7777 with the format:  DATEQUERY\0 (string)
5.    Whenever the application receives a DATEQUERY demand it answers to the source IP:port with a string message: DATE DD:MM:YYYY\0 (current date) using unicast.
