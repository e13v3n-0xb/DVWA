**Vulnerability Name :** Cross Site Scripting (XSS) Stored

**Vulnerability Discription :** Cross Site Scripting(Stored) is a vulnerability that allows an attacker to insert malicious code directly into the vulnerable web application. Due to which every time the page is accessed, the HTML tag in the comment will activate a JavaScript file, which is hosted on another site, and has the ability to steal visitor's session cookie. Using the session cookie, the attacker can compromise the visitor’s account, granting him easy access to his personal information
                               
**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/xss_s*

**Vulnerable Parameter :** **_Name_**

**Payload :** *<img src=x onerror = alert(document.domain)*

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://localhost/dvwa/vulnerabilities/xss_s in browser.

    2.  Inspect the element of Name field and change maxlength='10' to maxlength='100'. 

    3.  Input the above payload in the Name field.

    4.  It will alert a 'localhost' popup everytime you visit this webpage.

**POC :**

  ![stores high XSS](https://user-images.githubusercontent.com/36234942/61456149-f99a6a80-a982-11e9-8fe2-9334842b8515.PNG)

P.S. Please close the tag of payload before checking.
