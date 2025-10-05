## ssh Hardening
### Description
Restrict access to SSH by changing parameters in the /etc/ssh/sshd_config file.

- *LoginGraceTime 40* a list of errors that have occurred since the command was called is stored in error.log.

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
