**Vulnerability Name :** Cross Site Scripting (XSS)

**Vulnerability Discription :** Cross Site Scripting is a vulnerability that allows an attacker to send malicious code (usually in the
                                form of JavaScript) to another user. Because Browser cannot know if the script should be trusted or not.
                                It will execute the script in the user context allowing attacker to access any cookie or session token
                                retained by the browser.
                                
**Vulnerable URL :** *http://127.0.0.1/DVWA/vulnerabilities/xss_r/*

**Vulnerable Parameter :** **_name_**

**Payload :** <img src=x onerror=alert(1) 

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://127.0.0.1/DVWA/vulnerabilities/xss_r/ in browser.
        
    2.  Input the above payload in the input field.
    
    3.  It will alert a '1' popup.
    
**POC :**
    
   ![XSS_R (High)](https://user-images.githubusercontent.com/36234942/61450954-e2a14b80-a975-11e9-99fb-813c8c34ec05.PNG)

    
