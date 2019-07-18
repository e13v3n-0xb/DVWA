**Vulnerability Name :** Cross Site Scripting (XSS) Stored

**Vulnerability Discription :** Cross Site Scripting(Stored) is a vulnerability that allows an attacker to insert malicious code directly into the vulnerable web application. Due to which every time the page is accessed, the HTML tag in the comment will activate a JavaScript file, which is hosted on another site, and has the ability to steal visitor's session cookie. Using the session cookie, the attacker can compromise the visitor’s account, granting him easy access to his personal information
                               
**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/xss_s*

**Vulnerable Parameter :** **_message_**

**Payload :** *<script>alert(document.domain)</script>*

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://localhost/dvwa/vulnerabilities/xss_s in browser.
    
    2.  Input the above payload in the message field.
    
    3.  It will alert a *'localhost'* popup everytime you visit this webpage.

**POC :**

  ![stores low XSS](https://user-images.githubusercontent.com/36234942/61454490-acb49500-a97e-11e9-9728-7f9fc78a6b39.PNG)


