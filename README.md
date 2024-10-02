**1.** Open up the `Oracle Virtual Box`
![alt text](Images/image.png) 
**2,** Select `File` -> `Tools` -> `Network Manager`
![alt text](Images/image-1.png)
**3.** Select `Nat Networks`.

**4.** Select `Create` option and on the bottom panel enter your custom ipv4 address like `192.168.100.2/24`
![alt text](Images/image-2.png)
**5.** Click on `Apply` button

**6.** On the vbox, Select `Kali` -> `Settings`
![alt text](Images/image-3.png)
**7.** Now select `Networks` -> `Adapter1` -> `Attached to:` `NAT Network` and the name of Nat network will automatically written 
![alt text](Images/image-4.png)
**8.** Same approach for the ubuntu server and select adapter1 of ubuntu's network setting and voila!

**9.** Run both vms

**10.** Open up the terminal write `ifconfig` you will see the your set ip address

- **Ubuntu Server**
![alt text](Images/image-5.png)
- **Kali Linux**
![alt text](Images/image-6.png)

You can see the the ip address written right after `inet`

Now, if you select different adapters of 2 different machines while configuring the network (at stage 7) then that ip address will be in the `eth1` or in some other `eth` option

**11.** On ubuntu server write ping kali's ip and vice versa
- **Ubuntu Server**
![alt text](Images/image-7.png)
- **Kali Linux**
![alt text](Images/image-8.png)