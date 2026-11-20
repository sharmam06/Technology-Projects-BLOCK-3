# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

(Add screenshot here)

### Questions

1.  How many users exist on the system?
-There are total 36 users in the system including 2 normal users and 34 system accounts.
2.  Which accounts appear to be system accounts?
-Accounts such as root, daemon, nobody, sshd and messagebus.
3.  Why do operating systems create system accounts?
-To manage background services, improve security, restrict permissions and keep system processes separate from normal users.

### Reflection

Explain why understanding system users is important for cybersecurity.
-Understanding system users is important for cybersecurity because it  helps administrators control who can access the system and what actions they can perform. It protects sensitive information, prevents unauthorised access and reduces security risks.Different users have different permissions, which helps prevent misuse of administrator privileges.
------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)

### Questions

1.  Which processes are running as `root`?
-There are several processes running as 'root'such as;
-/sbin/init:Starts and manages system services. 
-kthreadd-:Manages kernel threads.
-kworker:Handles background kernel tasks.
2.  Why can processes running as root be dangerous?
-Root has the highest level of permission in Linux.Processes running as root can access and modify important system files,change security settings and control users. If a process has a security weakness,it could cause serious damage.
3.  What could happen if a malicious program ran with root privileges?
-Steal sensitive information and passwords.
-Delete or modify important system files.
-Install malicious software.
-Create unauthorised user accounts.
-disable security protections.

### Reflection

What did you learn about system processes and security?
-I learned that system processes keep the operating system running, and managing root permissions is important to prevent security risks and protect the computer from malicious programs.
------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot

(Add screenshot here)

### Questions

1.  Which ports are open?
-The first six ports are not connected and the last four are open.
2.  Which services appear to be listening?
-The last four tcp services appear to be listening.
3.  Why might open ports represent a security risk?
-Hackers try to acces sservices through open ports.
-Vulnerable services can be exploited.
-Attackers may steal sensitive information or disrupt services.

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
-Open ports increasres the attack surfaces because they provide entry points for attackers to access a computer or network.If services running on these ports have security weakness,hackers may exploit them to gain unauthorised access,steal data or damage the system.Therefore, closing unnecessary ports and securing essential services helps reduce security risks.
