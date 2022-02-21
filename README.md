# Java Group Chat Application

For compilation details please see the "ScreenShot IpOp.png".

Now it's time to clear some theoritical concepts.

A multicast host is specified by a class D IP address and by a standard UDP port number. Class D IP addresses are in the range 224.0.0.0 to 239.255.255.255, inclusive. The address 224.0.0.0 is reserved and should not be used. We can use IP addresses between 224.0.0.0 to 239.255.255.255.

*NOTE: port numbers 0 through 1023 are reserved

We need two threads in this application. One for accepting the user input (using the java.util.Scanner class) and the other for reading the messages sent from other clients. Hence I have separated the thread which does the reading work into ReadThreadclass. 

For leaving the group, any of the user can type in Exit to terminate the session.

The above program is executed on a single machine. Socket programming is meant for distributed programming. The same piece of code snippet when present on different machines which have Java installed can satisfy that requirement.
