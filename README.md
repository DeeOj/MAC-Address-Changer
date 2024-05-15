<h1> PROJECT: MAC ADDRESS CHANGER </h1>

<h2>  INTRO </p> </h2>
A MAC address is a unique identifier assigned to network devices, like computers or smartphones, for communication within a network. 
Since it's different for each device, spoofing or changing it on a software level can help during a penentration test to:

- Bypass Filters
- Impersonate other devices
- Increase Anonymity
<br></br>

<h2> OBJECTIVE </h2>
Write a Python script that, when executed in the terminal, prompts the user to input a network interface for which they want to change the MAC address,
along with the new MAC address to be applied. This script eliminates the need to manually disable and re-enable the network interface each time a MAC address change is required.
<br></br>

<h3> ENVIRONMENT & PROGRAMMING LANGUAGE USED </h3>  

- <b> Linux </b> <br/>
- <b> Python </b> 

<h3> IMPORTS </h3>

- <b> subprocess </b>: allows us to execute system commands
- <b> re </b> : enables us to work with complex string patterns

<h3> CHANGING THE MAC ADDRESS THROUGH TERMINAL </h3>
Let's explore how to achieve this via the terminal using a series of commands. This involves disabling the network interface whose MAC address we intend to change, and then re-enabling it after supplying a new address.
<br></br>

To begin, we'll utilize the "ifconfig" command to view the available interfaces.
<br><br/>

<p align="center">
<img src="https://imgur.com/IaD7o9P.jpg" height="90%", width="90%" alt ="Screenshot of running ifconfig on the terminal">
</p>


We can see Eth0 and lo.
<br/> "Eth0" is a virtual interface, with its MAC address highlighted. We will now alter its MAC address to one of our choosing. Say "08:07:ab:06:cd:05"

<p align="center">
<img src="https://imgur.com/XWjCaw6.jpg" height="90%", width="90%" alt ="">  
</p>

Now, we run the "ifconfig" command to see what has happened to the MAC address field for eth0. 
<br/> We see that the MAC address has changed to the one we specified.

<p align="center">
<img src="https://imgur.com/NDjNqbL.jpg" height="90%", width="90%" alt ="">  
</p>

<h3> AUTOMATING TASK USING PYTHON </h3>

I will be building this script and running it at different phases through the terminal.
Also, I will be writing my commands and arguments as a list, splitting them into a number of elements. This is so as to avoid using the "shell=True" Parameter in the subprocess function, which has the potential to grant users the ability to enter Linux commands, which can actually be executed on the system. In simpler terms, to avoid creating a vulnerability supcestible to shell injection attacks.

<p align="center">
<img src="https://imgur.com/Pp3OVgs.jpg" height="90%", width="90%">  
</p>



I navigated to the directory where my Python file resides and executed it in the terminal. 
So far, the script prompts a user to input the network interface and the desired MAC address, but does not change it yet.

<p align="center">
<img src="https://imgur.com/pToLQ5N.jpg" height="90%", width="90%">  
</p>

<p align="center">
<img src="https://imgur.com/mVI6SAj.jpg" height="90%", width="90%">  
</p>

After inserting the new address, it prints the statement I specified in the code.
<p align="center">
<img src="https://imgur.com/s2dFM8x.jpg" height="90%", width="90%">  
</p>

Now, for the iterative part ⬇️
<p align="center">
<img src="https://imgur.com/cwW3vkm.jpg" height="90%", width="90%">  
</p>

Now, when executed, it does change the MAC address.
<p align="center">
<img src="https://imgur.com/klDqM0e.jpg" height="90%", width="90%">  
</p>

<h3> PARSING </h3>
I have now imported "re" module and cleaned up my code.
<br><br/>

<p align="center">
<img src="https://imgur.com/VAZ6jUT.jpg" height="90%", width="90%">  
</p>

Final Ouput:

<p align="center">
<img src="https://imgur.com/pCerdH1.jpg" height="90%", width="90%">  
</p>

<h2> CONCLUSION </h2>

The "MAC Address Changer" project demonstrates the power of automation in network configuration tasks. By leveraging Python scripting and subprocess execution, I've developed a tool capable of dynamically changing MAC addresses on Linux systems. This project not only enhances efficiency but also contributes to my cybersecurity awareness by showcasing the potential vulnerabilities associated with MAC address spoofing if built in a certain way.

<br></br>

<p align="center">
<b> Thank you for joining me on this journey. </b>
</p>
