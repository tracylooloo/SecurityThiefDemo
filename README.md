# Final Project - Physical Computing and the Internet of Things

This is a template for your final project documentation.  Please replace <content like this> with your own.  For help with the syntax of Github markdown, visit: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

*Name:*  Tracy Lu

*Date:* December 2017

## Project:  Security Thief

< 2 - 3 sentence brief description / abstract of your project>
The purpose of my project was to display potential attacker effects and inspire caution about the use of IOT and cloud-based voice assistant devices, especially ones linked to private information and important smart home hardware. This was done by creating a series of Alexa Skills that involve private data and hardware. 


### Detailed Project Description

#### Background Information:
 The voice assistant device I used was the Echo Dot. Alexa is the cloud voice service and Echo is the hardware device consisting of a microphone array capable of beaming and noise cancellation which respond to the wake word “Alexa”.
It's interesting how much is accessible through Alexa and the Amazon eco system . For example, to make the Alexa Skill, I used my AWS account which is linked to my Alexa Skills Developer account, Amazon Alexa account, Amazon.com account, Zappos account, which means that if someone hacked into my account through my Echo they would have access to my credit card, buying items, the things that I’m hosting on AWS, the hardware and appliances that the voice assistant is connected to, and other private information. Also, most people have their voice assistants in an open mode, meaning that anyone can talk to it and the Echo will respond. In addition, a couple months ago I read an article about how some hackers are using high frequency recordings that the Echo’s hardware can pick up and execute but that humans can’t hear, allowing them to secretly gain access to information without the owner knowing at all. Voice Assistants are becoming increasingly popular especially in homes and other hardware devices. People are trusting voice assistants for lights, cameras, locks, etc. and personal information due to the convenience that it offers.

I wanted to demonstrate these themes with three Alexa Skills representing three different scenarios or stories.

##### Alexa Skill One: Phone trigger 
An attacker could secretly ask the Echo to call the owner and send an evil message. The Echo does not record the voice or recording of the attacker, because the Alexa voice service only keeps the JSON objects processed from the voice commands. This allows the attacker to have anonymity and makes it difficult to track or trace back the attacker. I set up an Alexa Skill to demonstrate this, which assumes that the owner has settings on his or her device that knows the owner's phone number and allows it to be messaged, which people usually enable for convenience purposes. The attacker will ask "Alexa trigger call my phone" and the phone message sent is "Send $2000 to xyzhacker paypal account otherwise you will die tomorrow". 


### Technical Description

< Explain the "how" of your project.  What are the hardware components?  What are the software components?  How do they interact with each other? >

< You can also explain the development process here >
##### Alexa Skill One: Phone trigger 
This was made by linking my Amazon Alexa account to an IFTTT applet and adjusting the settings in the IFTTT applet. 


#### Hardware Wiring Diagram

![Wiring Diagram](images/WiringDiagram.png)
< Insert Picture and explanation of Your Wiring Diagram here >

#### Code

< Explain your code.  You might include code snippets, either `inline` or
```c++
//Multiline
bool photon_fun = TRUE;
```
You should link to your full code, either included in the repository (e.g. [my_code.ino](code/my_code.ino)  or to the Shared Revision in your Particle IDE. >




### Design / Form

< Explain the device's form, the aesthetic choices made and how they relate to the concept/function the device is intended to engage >

< include photos of your device >
The 3D printed enclosure represents a theif. I modeled the enclosure specific to the dimensions of the Echo Dot and left the top hollow for acoustic effects. I also made sure there was enough of a gap between the edge of the enclosure and the outer array of microphones. 

[Video](https://drive.google.com/file/d/17v_A_foWOlvpR0w_vulE1JuxNCLYIStu/view?usp=sharing) of one of the Alexa Skills:


### Evaluation / Reflection

< What is your own evaluation of your project?   What did you learn through this project?  What would you do differently in the future? >
I was not expecting to have issues with connecting my pi to the Alexa cloud service, and was surprised by the firewall and restrictions implemented by Duke OIT. This did make me more aware of the security and "behind the scenes" of Duke networks, and how different it is from a home network, which actually helped me prove my of my point regarding the vulnerability of smart home devices. Although my LED strip couldn't be connected on Duke's WiFi, I plan to bring back the set up over winter break and try it in my home. 
