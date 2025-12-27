*This project has been created as part of the 42 curriculum by : <Aagodim>*

# NetPractice

## Description :

    NetPractice is a project that introduces a new concepts and things in the 42 curriculum aside from the coding area, this project focuses more on the networking side and how data are sent from a device A to a device B locating either on the same area (house, company) or worldwide!

    In this project you will learn about :

    * What's a network ?
    * Differences between hubs, switches, and routers
    * How does networking works? (TCP/IP or OSI model) ?
    * What's an IP address/subnet mask/ gateway and how does subnetting works 

    a **Network** is a group of two or more devices that can communicate amongst each other, by communicating we mean the possibility of sending and receiving data between these devices. Each device has an Ip address, a subnet mask and default gateway which we will get through later!

### Hub, switching and routing

    * Hub is a device that connects the devices but it doesn't know the destination where it should send the data to, that's why it works on the layer 1.

    * Switch unlike the hub works on the layer 2 which is categorized with Mac addresses that the switch uses to decide where to send the data.

    * Unlike these two the router connects the networks rather than devices and decides the best path for it take, it uses IPS to make decisions and works on the layer 3.

### Network models and layers

    To know better how data moves from a device to another one, we've got two models, TCP/IP and OSI.

    * TCP/IP model is the practical model that we use on the internet and it has 5 layers

      1/ Application (HTTP, HTTPS, DNS, DHCP)
      2/ Transport (TCP, UDP)
      3/ Network (IP)
      4/ Data Link (Ethernet, ARP)
      5/ Physical (cables, radio waves, fiber)

    * Osi model is more of a theoretical model that explains and makes undestands more the networking that's why it has 7 layers!!

      1/ Application
      2/ Presentation
      3/ Session
      4/ Transport
      5/ Network
      6/ data link
      7/ physical

### Ip addressing and subnetting

    * Ip stands for Internet protocol, uniquely identifies every device on the internet and without one there’s no other way to contact them and an IP address got two important parts, which are:

        **The Network ID**
        **The Host ID**
    
    * If the destination data you will send to is outside your local network then the **Default Gateway** steps in and without you cannot access to the other   networks, for example let's your device A wanna send some data to device B with an ip of (1.1.1.1) the broadcast will shout in your network looking for the device with that ip address and zero answer found then the default gateway takes place to look outside your network!

    * Subnetting is the idea of dividing a large network into smaller networks **How**? Using the subnet mask that's accompanied with the ip of the address, it's also helps you know which part is for the network (you can't touch) and the host part (which you can choose an ip from and give it yo your device)

    ####How to subnet :
        
        Right now most people still use the IPv4 mode since its what the internet uses, it uses 32 bit addresses and it each octet of it written in a decimal way ranged between 0-255 (example 192.168.1.1) to know which part is the network/host you look at the subnet mask which as I said before is in the network settings, let's say our subnet mask is 255.255.255.0 (which also can be written like /24) usually you convert the decimal numbers into binaries and you go from there (1bits represents the network and 0s represents the host)

        255.255.255.0 = 11111111.11111111.11111111.00000000 which mean 192.168.1 -> network and the 0 is for the host. And to know how many ip addresses are left to use either you do 255 - 0 (the ip host number) - 2 (network ip + broadcast ip) = 254 or 2 to the power of (32 - 24) - 2 = 254

        **WHY?**

        1/ Reduce the broadcast traffic
        2/ Improve performance
        3/ Simplify the network management


## Instructions :

    This project doesnt need any compilation nor execution, you only clone the git repository folder and you will check that there're 10 .json files (the levels you will have to complete in the training mode), how so? at first you clone the project's winrar in your intra and extract it **tar -xvzf /path/to/yourfile.tgz** in your Desktop (or tha location you choose to upload the project in), after that you will notice a folder named after your project, inside the folder you will see different files but your main focus is the "index.html" file which you will run (works better on Brave!) the UI is quite simple to understand, there're two modes evaluating/training!

    **Training** : you go up level by level and on each one you learn a new concept and skill until you complete 10 levels!
    **Evaluatig** : three random levels from 6 to 10 will be offered to be solved in 15 minutes!

    When you're on one of the modes above you will a notice a figuration of devices with a placeholder (this is where you will put the correct IP address to connect the networks), once you finish you will see at the top {CHECK} button which will evaluate your configuration if it's correct two more buttons will poop {GET MY CONFIG} which will download your json file that has that level and {NEXT LEVEL} which is obvious haha! Once you complete the 10 levels, the files you download will be placed in a folder and pushed to your intra!

## Ressources :

    As I mentioned before, in this project you will learn about lot of things, at first you will look for articles, document or youtube video to get a clear idea of what you're getting into (not AI, it ruins the joy :D)

    On the theory part this playlist will enrich your knowledge :

    1/ https://www.youtube.com/watch?v=tSodBEAJz9Y&list=PLF1hDMPPRqGxpYdo0ctaa7MxfOi9vjs1u (Basically how network works)

    2/ https://www.youtube.com/watch?v=s_Ntt6eTn94 (Subnet mask)

    3/ https://www.youtube.com/watch?v=5WfiTHiU4x8&list=PLIhvC56v63IKrRHh3gvZZBAGvsvOhwrRF&index=1 (Subnetting)

    4/ https://medium.com/@imyzf/netpractice-2d2b39b6cf0a (general idea on the project by a fellow student)

    When it comes to the mathematical part on how to deal with subnetting and overlapping of Ip range you will have to face and deal with, AI isn't really gonna help you with much but it can clarify the theoretical parts and networking concepts.
