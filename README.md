# Reverse-Engineering-Tenda-CP3


Hello, today im going to teach  you how to reverse engineer your Tenda CP3 camera.

First you need to connect your ip camera to your wifi. Then with Nmap (https://github.com/nmap/nmap) you can do a fast scan (nmap -F your_camera_ip)

![image_2022-04-17_191717940](https://user-images.githubusercontent.com/64932654/163725335-ca33bbaa-51ba-4e0a-96f0-bcd1ccd92082.png)


We can see that 4 ports are showing up: 
Telnet(terminal network), An unknown service, h323hostcallsc(H323 Host Call Secure), sd(	Session Director)

From that we can try to connect to the camera via Telnet:

![image_2022-04-17_192005782](https://user-images.githubusercontent.com/64932654/163725417-2a241acb-85a7-4565-808d-609476ccdb4f.png)

I didnt try to bruteforce it but the login admin and password admin didnt worked so I went ahead. 
I started 
