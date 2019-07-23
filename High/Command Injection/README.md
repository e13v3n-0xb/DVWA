**Vulnerability Name :** **Command Injection Vulnerability**

**Vulnerability Description :** Command injection is an attack in which the goal is execution of arbitrary commands on the host operating system via a vulnerable application. Command injection attacks are possible when an application passes unsafe user supplied data to a system shell. In this attack, the attacker-supplied operating system commands are usually executed with the privileges of the vulnerable application. Command injection attacks are possible largely due to insufficient input validation.
                                
An attacker could run arbitrary system-level OS commands on the application server host. Depending on the application’s OS permissions, these could include:

· File actions (read / create / modify / delete)

· Open a network connection to the attacker’s server

· Start and stop system services

· Modify the running application

· Complete server takeover

**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/exec/*

**Vulnerable Parameter :** *ip*

**Payload :** *[IP] |dir*

**How to reproduce this vulnerability :**

     1.  Request this URL: http://localhost/dvwa/vulnerabilities/exec/ in browser.

     2.  Input the above payload in the 'ip' input field.

     3.  It will execute the given arbitary command.
     
**POC :**
    
    **Vulnerability Name :** **Command Injection Vulnerability**

**Vulnerability Description :** Command injection is an attack in which the goal is execution of arbitrary commands on the host operating system via a vulnerable application. Command injection attacks are possible when an application passes unsafe user supplied data to a system shell. In this attack, the attacker-supplied operating system commands are usually executed with the privileges of the vulnerable application. Command injection attacks are possible largely due to insufficient input validation.
                                
An attacker could run arbitrary system-level OS commands on the application server host. Depending on the application’s OS permissions, these could include:

· File actions (read / create / modify / delete)

· Open a network connection to the attacker’s server

· Start and stop system services

· Modify the running application

· Complete server takeover

**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/exec/*

**Vulnerable Parameter :** *ip*

**Payload :** *[IP] | dir*

**How to reproduce this vulnerability :**

     1.  Request this URL: http://localhost/dvwa/vulnerabilities/exec/ in browser.

     2.  Input the above payload in the 'ip' input field.

     3.  It will execute the given arbitary command.
     
**POC :**
    
   ![command injection medium](https://user-images.githubusercontent.com/36234942/61731891-0d3a3c80-ad9a-11e9-9d78-e02d62e665ad.PNG)
