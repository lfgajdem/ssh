## ssh Hardening
### Description
Restrict access to [SSH](https://www.openssh.com/) by changing parameters in the */etc/ssh/sshd_config* file.

- **LoginGraceTime 40** The time after which the server disconnects if the user has not successfully logged in.
- **StrictModes yes** Specifies whether sshd should check file modes and ownership of the user's files and home directory before accepting login.
- **MaxAuthTries 3** Specifies the maximum number of authentication attempts permitted per connection. When the login failure count reaches half the number, error messages will be written to the syslog file detailing the login failure.
- **PermitRootLogin no** Disables direct root access.
- **AllowUsers	User1 User2@HOST** User 1 can log in from any computer. User 2, however, can only log in from the HOST computer.
- **PermitEmptyPasswords no** Deny login access to accounts with empty password fields.
- **Banner /etc/banner_ssh** The contents of the file will be printed to the client before login.

<figure>
   <figcaption><sub>Fig.1 There were failed login attempts by the following unauthorized users: root, admin, and administrator. </sub></figcaption>
   <img src="./images/ssh01.png" 
   alt="Unauthorized users: root, admin, and administrator." 
   title="Unauthorized users">
</figure>

> [!IMPORTANT]
> Do not use default usernames such as "root," "admin," or "administrator."

<figure>
  <figcaption><sub>Fig.2 A successful connection to the server has been established.</sub></figcaption>
  <img src="./images/ssh02.png" 
   alt="Successful connection." 
   title="Successful connection has been established.">
</figure>
