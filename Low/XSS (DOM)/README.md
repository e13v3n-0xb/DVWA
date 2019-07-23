**Vulnerability Name :** DOM Cross Site Scripting (XSS) 

**Vulnerability Discription :** DOM Based XSS simply means a Cross-site scripting vulnerability that appears in the DOM (Document Object Model) instead of part of the HTML. In reflective and stored Cross-site scripting attacks you can see the vulnerability payload in the response page but in DOM based cross-site scripting, the HTML source code and response of the attack will be exactly the same, i.e. the payload cannot be found in the response. It can only be observed on runtime or by investigating the DOM of the page.

After the malicious code is executed by page, attacker can simply exploit this DOM based cross-site scripting vulnerability to steal the cookies from the user's browser or change the behaviour of the page on the web application as attacker like.


**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/xss_d/*

**Vulnerable Parameter :** *default*

**Payload :** *<script>alert(document.domain)</script>*

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://localhost/dvwa/vulnerabilities/xss_d/ in browser.
        
    2.  Choose a language and click on Select button.
    
    3.  Enter the above payload in URL in default parameter.
    
    4.  It will alert a 'localhost' popup.
    
**POC :**

   ![dom low](https://user-images.githubusercontent.com/36234942/61734642-f0086c80-ad9f-11e9-949f-7f318f7ede17.PNG)
