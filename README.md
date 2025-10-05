## ssh Hardening
### Description
Restrict access to [SSH](https://www.openssh.com/) by changing parameters in the /etc/ssh/sshd_config file.

- **LoginGraceTime 40** The time after which the server disconnects if the user has not successfully logged in.
- **StrictModes yes** Specifies whether sshd(8) should check file modes and ownership of the user's files and home directory before       accepting login.  
- **PermitRootLogin no** Disables direct root access.
- **Banner /etc/banner_ssh** the contents of the file will be printed to the client before login.

<figure>
   <figcaption><sub>Fig.1 Here is an example of a user who does not exist.</sub></figcaption>
   <img src="./images/ssh01.png" 
   alt="Here is an example of a user who does not exist." 
   title="User not exist">
</figure>

<figure>
  <figcaption><sub>Fig.2 The system detected an attempt to log in as a guest user.</sub></figcaption>
  <img src="./images/ssh02.png" 
   alt="The system detected an attempt to log in as a guest user." 
   title="guest user">
</figure>
