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
- <b> Re </b> : enables us to work with complex string patterns

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





















<p align="center">
  
</p>
