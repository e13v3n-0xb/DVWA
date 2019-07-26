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

**Malicious File :** *shell.php*

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://localhost/dvwa/vulnerabilities/upload/ in browser.
        
    2.  Click on 'browse' button and select the shell.php file 
    
    3.  Now ulpoad the php file. it will get uploaded directly.
    
**POC :**

  ![upload low](https://user-images.githubusercontent.com/36234942/61954987-bb7ef580-afd7-11e9-8431-d5c3436b6a98.PNG)

  
