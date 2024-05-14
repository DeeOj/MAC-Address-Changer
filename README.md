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

<h3> ENVIRONMENT USED </h3>  
Linux 

<h3> IMPORTS </h3>

- <b> subprocess </b>: allows us to execute system commands
- <b> Re </b> : enables us to work with complex string patterns
