## SelectiveRepeat

1. Clone the code and cd to ARQProtocols/Selective/.

2. Make sure you have python installed on your machine. To check the version type `python --version` It should tell you that you have version 2.7.

3. Start the Receiver by the following command: `python Receiver.py 7765 output.txt 0.05`

In the above command the 7765 will be the wellknown port on which the receiver is running, output.txt is the file where the file data will be stored and 0.05 will 
be the error probability of the packet lost.

4. Start the Sender by the following command: `python Sender.py 152.46.19.251 7765 rfc123.txt 64 500`

In the above command the 152.46.19.251 will be the receiver ip address and 7765 will be the wellknown port of the receiver, rfc123.txt will be the path where the rfc is 
located which needs to be transferred, 64 is the window size and 500 will be the MSS.

5. You can use the rfc file from `ARQProtocols/GoBack/` if you dont have one.
