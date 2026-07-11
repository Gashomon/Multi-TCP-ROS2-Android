## **MULTI CLIENT ROS2 to Anroid TCP Communication via Python**

A basic multi-client TCP link for one server and multiple connections sharing one ROS2 publisher to send info.

Based from [mirellameelo](https://github.com/mirellameelo/ROS_2_ANDROID), designed to receive tcp logs from android devices conencted. I did not include here the app side since it is focused on the communication method via passing plain text over TCP. 

Translation the TCP logic into Python with original guide from [wittcode's blog](https://blog.wittcode.com/blogs/python-socket-programming-multiple-clients-chat.) (Sadly, domain seemed to be removed) but another reference is from [Real Python](https://realpython.com/python-sockets/#running-the-multi-connection-client-and-server).


### DEPENDENCIES
- ROS2 (Humble Hawksbill)
- ANDROID STUDIO
- PYTHON 3


### INSTALLATION
[ROS 2 INSTALLATION](https://docs.ros.org/en/humble/Installation.html)
[ANDROID STUDIO EMULATOR](https://developer.android.com/studio/run/emulator)


### HOW TO RUN
1. Run on the ROS2 system: [android_server.py](https://github.com/Gashomon/Simple-ROS-Android-TCP-2-way-Comm/blob/main/src/rosandroid/android_server.py) 
2. Run your Android app. It needs to automatically search for the ROS2 server and attempt to establish connection with it.
3. You can send any plain text message and the server will translate the message to the ROS2 system as a publisher.
4. Send 'bye' to disconnect with the ROS2 server.
