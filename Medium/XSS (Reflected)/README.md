**Vulnerability Name :** Cross Site Scripting (XSS)

**Vulnerability Discription :** Cross Site Scripting is a vulnerability that allows an attacker to send malicious code (usually in the
                                form of JavaScript) to another user. Because Browser cannot know if the script should be trusted or not.
                                It will execute the script in the user context allowing attacker to access any cookie or session token
                                retained by the browser.
                                
**Vulnerable URL :** *http://127.0.0.1/DVWA/vulnerabilities/xss_r/*

**Vulnerable Parameter :** **_name_**

**Payload :** *<sCRipT>alert(document.domain)</sCRiPT>*

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://127.0.0.1/DVWA/vulnerabilities/xss_r/  and then fill the input field and make a 
        request in intercept with BurpSuite.
        
    2.  Change the name parametre value to the payload.
    
    3. it will alert a '127.0.0.1' popup.
    
**POC :**
    
   ![XSS_R (Medium)](https://user-images.githubusercontent.com/36234942/61449504-b89a5a00-a972-11e9-94d8-cd9128a4f9f6.PNG)



