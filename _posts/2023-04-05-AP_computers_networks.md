---
toc: true
comments: true
layout: post
title: Computers and Networks (Unit 4)
description: Add Definitions from Unit 4 Computer Systems and Networks
image: /images/apcsp.png
categories: []
type: ap
week: 29
---

## Requirements
> Work through College Board Unit 4... blog, add definitions, and pictures.  Be creative, for instance make a story of Computing and Networks that is related to your PBL experiences this year.


### How a Computer Works
> As we have learned, a computer needs aa program to do something smart.  The sequence of a program initiates a series of actions with the computers Central Processing Unit (CPU). This component is essentially a binary machine focussing on program instructions provided.  The CPU retrieives and stores the data it acts upon in Random Access Memory (RAM). Between the CPU, RAM, and Storage Devices a computer can work with many programs and large amounts of data.

List specification of your Computer, or Computers if working as Pair/Trio
Processor	AMD Ryzen 5 5625U with Radeon Graphics, 2301 Mhz, 6 Core(s), 12 Logical Processor(s)
- <b>Processor GHz</b>: 3.3 GHz(Clock speed of a computer's CPU)
- <b>Memory in GB</b>: 16 GB 
- <b>Storage in GB</b>: 246 GB 
- <b>OS</b>: Microsoft Windows 11 Home


Define or describe usage of Computer using Computer Programs. Pictures are preferred over a lot of text.  Use your experience.
- <b>Input devices</b>: Hardware components that allow users to interact with a computer by providing it with data or instructions. Ex. Mouse, Touchscreen, Microphone, Webcam
- <b>Output devices</b>: Hardware components that display data processed by a computer to the user. Ex. Monitor, Printer, Projector
- <b>File</b>: Collection of data/info that is stored in a specific location in a computer. Can contain text, images, audio, video, etc.
- <b>Program Code</b>: Written set of instructions that tells your computer how to perform a specific task. It is written in a programming language and compiled into a program file.
- <b>Processes</b>: Individual programs or tasks that are running on your computer’s operating system.
- <b>Ports</b>: Communication endpoints that allow data to be exchanged between devices or applications in a computer network.
- <b>Data File</b>: File that contains data or information that can be used by a program. Examples include text files, images, and spreadsheets.
- <b>Inspect Running </b>: The process of examining the code that is currently executing on your computer to troubleshoot or debug issues.
- <b>Inspect Variables</b>: Process of examining the variables, or named storage locations, in a program’s code to understand how they are being used and how they are affecting the program’s behavior.

![Diagram]({{site.baseurl}}/images/firstpic.png)
![Computer Hardware]({{site.baseurl}}/images/cpu.jpeg)


### The Internet
> Watch/review College Board Daily Video for 4.1.1

- Essential Knowledge
    - A computing device is a physical artifact that can run a program. Some examples include computers, tablets, servers, routers, and smart sensors.
    - A computing system is a group of computing devices and programs working together for a common purpose.
    - A computer network is a group of interconnected computing devices capable of sending or receiving data.
    - A computer network is a type of computing system. 
    - A path between two computing devices on a computer network (a sender and a receiver) is a sequence of directly connected computing devices that begins at the sender and ends at the receiver.
    - Routing is the process of finding a path from sender to receiver.
    - The bandwidth of a computer network is the maximum amount of data that can be sent in a fixed amount of time.
    - Bandwidth is usually measured in bits per second

- Complete Vocabulary Matching Activity.  Incorporate this into your learnings from year.  To analyze measure path and latency use `traceroute` and `ping` commands from Linux Terminal.  
    - A <b>Path</b>: Sequence of directly connected computing devices that begins at sender and ends at receiver 
    - E <b>Route</b>: Process of finding a path from sender to receiver 
    - B <b>Computer System</b>: A group of computing devices working together for a joint purpose 
    - C <b>Computer Device</b>: Physical artifact that can run a program. Ex. Computers, tablets, servers, routers, etc. 
    - D <b>Bandwidth</b>: Max amount of data that can be sent in a fixed amount of time on a computer network 
    - F <b>Computer Network</b>: Type of computing system. A group of interconnected computers that can send and recieve data to each other 
    - <mark>Extra to know</mark>: Computers talk through <b>packet Switching</b>: The message (file) is broken up into packets and send in any order. The packets are reassembled by the recipient’s device. A <b>packet</b> is a small amount of data sent through network, contains source and destination info
![Path and Routing]({{site.baseurl}}/images/pathandrouting.png)

> Watch/review College Board Daily Video 4.1.2

- Complete True of False Questions

- Essential Knowledge
    - The internet is a computer network consisting of interconnected networks that use standardized, open (nonproprierary) communication protocols.
    - Access to the internet depends on the ability to connect a computing device to an internet connected device.
    - A protocol is an agreed-upon set of rules that specify the behavior of a system.
    - The protocols used in the internet are open, which allows users to easily connect additional computing devices to the internet.
    - Routing on the internet is usually dynamic; it is not specified in advance
    - The scalability of a system is the capacity for the system to change in size and scale to meet new demands.
    - The internet was designed to be scalable
    - Information is passed through the internet as a data stream. Data streams contain chunks of data, which are encapsulated in packets. 
    - Packets contain a chunk of data and metadata used for routing the packet between the origin and the destination on the internet, as well as for data reassembly.
    - Packets may arrive at the destination in order, out of order, or not at all
    - IP, TCP and UDP are common protocols used on the internet.
    - The world wide web is a system of linked pages, programs, and files.
    - HTTP is a protocol used by the world wide web
    - The world wide web uses the internet

<mark>Extra Notes</mark>

![Model]({{site.baseurl}}/images/model.png)
- <b>Network Access</b>: Hardware (ex. Internet cable, wifi cable) 
- <b>Internet</b>: Packers, Sender and receiver IP, metadata for routing information
- <b>Transport</b>: TCP (error checking and error recovery very slow, 3-way handshake to verify delivery) & UDP (error checking, discards erroneous packets) 
- <b>Application</b>: web services, domain name service, http/https(http w/ security)
- <b>World-Wide Web</b>: linked data pages, NOT Internet 

- Go over AP videos, vocabulary, and essential knowledge.  Draw a diagram showing the internet and its many levels. A preferred diagram would using your knowledge of frontend, backend, deployment, etc.  Picture would highligh vocabulary by illustration. The below illustration have some ideas

![Full Stack]({{site.baseurl}}/images/fullstack.png)

- <b>Complete True of False Questions</b>
1. T 
2. F
3. F
4. T
5. F
6. F
7. T

- Often we draw pictures of machines communicating over the Internet with arrows.  However, the real communication goes through protocol layers and the machine and then is trasported of the network.   For College Board and future Computer Knowledge you should become familiar with the following ...

```
     User Machine  <---> Frontend Server <---> Backend Server
    +-----------+         +-----------+         +-----------+
    |  Browser  |         |  GH Page  |         |   Flask   |
    +-----------+    ^    +-----------+    ^    +-----------+
    |    HTTP   |    |    |    HTTP   |    |    |    HTTP   |
    +-----------+    |    +-----------+    |    +-----------+
    |    TCP    |    |    |    TCP    |    |    |    TCP    |   
    +-----------+    |    +-----------+    |    +-----------+
    |     IP    |    V    |     IP    |    V    |     IP    |
    +-----------+         +-----------+         +-----------+
    |  Network  |  <--->  |  Network  |  <--->  |  Network  |
    +-----------+         +-----------+         +-----------+
```

The "http" layer is an application layer protocol in the TCP/IP stack, used for ***communication between web browsers and web servers***. It is the protocol used for transmitting data over the World Wide Web.

The "transport" layer (TCP) is responsible for providing reliable data transfer between applications running on different hosts.  The TCP protocol segments the data into smaller ***chunks called "segments"***. Each segment contains a sequence number that identifies its position in the original stream of data, as well as other control information such as source and destination port numbers, and checksums for error detection.

The "ip" layer is responsible for packetizing data received from the TCP layer of the protocol stack, and then ***encapsulating the data into IP packets***. The IP packets are then sent to the lower layers of the protocol stack for transmission over the network.

The "network" layer is responsible for ***routing data packets between networks*** using the Internet Protocol (IP). This layer handles tasks such as packet addressing and routing, fragmentation and reassembly, and ***network congestion*** control.


### Fault Tolerance
> Watch both Daily videos for 4.2
- <b>NOT fault tolerant</b>: Doesn’t use many resources, Failure in one network = fatal 
- <b>Fault tolerant</b>: Redundant and uses more resources. But even if one path goes down, a device can communicate with all other devices. Makes network stronger!


- <b>Complete the network activity, summarize your understanding of fault tolerance.</b>
Fault tolerance is a network’s ability to withstand disconnections. Networks use many interconnected nodes to guarantee that no one or two interrupted connections can take down a system. You can tell if a network is fault tolerant by checking that even if one path goes down, every device can communicate with all other devices. 

### Parallel and Distributed Computing
> Review previous lecture on Parallel Computing and watch Daily vidoe 4.3.  Think of ways to make something in you team project to utilize Cores more effectively.  Here are some thoughts to add to your story of Computers and Networks...

<mark>Notes</mark>
- Computer tasks: balance tasks so all CPUs used evenly and fully 
    - System tasks: scheduling what to do next, managing hardware, working with network
    - User tasks: executing programs that the user has selected
- <b>Sequential Computing</b>: Tasks are done one after another 
- <b>Parallel Computing</b>: program broke into multiple smaller sequential computing programs, some at the same time! 
    - Normally on same computer
    - Hardware driven, faster operations, data driven, 
- Compare efficiency by execution time
- Speed up time: time to complete task sequentially / time to complete task in parallel 
- <b>Distributed Computing</b>: sending of tasks from one computer to another, mix of sequential and parallel 
    - Solve problems that can’t be done with one computer bc of processing time/storage Ex. google web search
    - Needs a network 

- What is naturally Distributed in Frontend/Backend archeticture?  

- Analyze this command in Docker: ```ENV GUNICORN_CMD_ARGS="--workers=1 --bind=0.0.0.0:8086"```.   Determine if there is options are options in this command for parallel computing within the server that runs python/gunicorn.  Here is an [article](https://medium.com/building-the-system/gunicorn-3-means-of-concurrency-efbb547674b7)


> Last week we discussed parallel computing on local machine.  There are many options.  Here is something to get parallel computing work with a tool called Ray.
- Review this [article](https://www.anyscale.com/blog/writing-your-first-distributed-python-application-with-ray)...  Can you get parallel code on images to work more effectively?  I have not tried Ray.

- Code example from ChatGPT using squares.  This might be more interesting if nums we generated to be a lot bigger.

```python
import ray

# define a simple function that takes a number and returns its square
def square(x):
    return x * x

# initialize Ray
ray.init()

# create a remote function that squares a list of numbers in parallel
@ray.remote
def square_list(nums):
    return [square(num) for num in nums]

# define a list of numbers to square
nums = [1, 2, 3, 4, 5]

# split the list into two parts
split_idx = len(nums) // 2
part1, part2 = nums[:split_idx], nums[split_idx:]

# call the remote function in parallel on the two parts
part1_result = square_list.remote(part1)
part2_result = square_list.remote(part2)

# get the results and combine them
result = ray.get(part1_result) + ray.get(part2_result)

# print the result
print(result)

```
