##A multicast video/webcam streaming program written in python. The program will implement a custom UDP protocol with some addition features 
(sequence numbers, source and destination in the protocol header). The data in the payload will need to be encrytped using a simple symetric key encryption scheme.

retransmitted and duplicated packets should be dropped, but out of order packets need to be rapidly sorted or otherwise dropped to ensure smoother video feed.

# How to use it ?

In order to test it, run the server :

    python3 server.py --port 10080 

In another tab, start the client :

    python3 client.py --host localhost --port 10080

Pressing 'q' on the client side within the CV2 window will isue a quit command to the client and server.

Isaiah
Thanks.