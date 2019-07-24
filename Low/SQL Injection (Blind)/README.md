**Vulnerability Name :** **SQL Injection (Blind)**

**Vulnerability Discription :** Blind SQL injection is identical to normal SQL Injection except that when an attacker attempts to exploit an application, rather then getting a useful error message, they get a generic page specified by the developer instead. This makes exploiting a potential SQL Injection attack more difficult but not impossible. An attacker can still steal data by asking a series of True and False questions through SQL statements.

**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/sqli_blind/*

**Vulnerable Parameter :** *id*

**Payload :** *1' OR 1 = 1#*

**How to reprouce this Vulnerability :**

    1.  Request this URL: http://localhost/dvwa/vulnerabilities/sqli_blind/ in browser.
        
    2.  Input the above payload in the 'id' field.
    
    3.  It will show the information of users stored in database.
    
**POC :**
   
   ![sql blind low](https://user-images.githubusercontent.com/36234942/61800591-ec7def80-ae4a-11e9-8c1c-e75e698e7265.PNG)
