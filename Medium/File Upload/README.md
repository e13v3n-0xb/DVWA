**Vulnerability Name :** **File Upload Vulnerabilities** 

**Vulnerability Discription :** Various web applications allow users to upload files (eg images, music files etc). The uploaded files can create risk if not handled in a secure way. Depending on the how the file is processed and where it is stored the impact of the file upload vulnerability may vary.
     
Impact:
- The attacker can get a web shell and execute various commands, browse system files and browse local resources etc.
- Make a phishing page in the website.
- Make a permanent XSS in the website.
- Uploaded sensitive files might be accessible by unauthorized people.
- Uploaded files might trigger vulnerabilities in broken libraries/applications on the client side.
- Uploaded files might trigger vulnerabilities in broken libraries/applications on the server side.
- Uploaded files might trigger vulnerabilities in broken real-time monitoring tools.

**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/upload/*

**Malicious File :** *shell.jpg*

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://localhost/dvwa/vulnerabilities/upload/ in browser.
        
    2.  Click on 'browse' button and select the 'shell.jpg' file and intercept the request in burpsuite. 
    
    3.  Now, alter the 'shell.jpg' to 'shell.php'.
    
    4.  Forward the request. The malicious file will get uploaded.
    
**POC :**
  
  ![file upload med](https://user-images.githubusercontent.com/36234942/61954988-bc178c00-afd7-11e9-94d8-1b6b2e6e3d73.PNG)


  
