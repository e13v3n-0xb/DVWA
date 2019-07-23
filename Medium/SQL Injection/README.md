**Vulnerability Name :** **SQL Injection**

**Vulnerability Description :** SQL injection is considered a high risk vulnerability due to the fact that can lead to full compromise of the remote system. if an application is vulnerable to SQL injection then it allows attackers to interact with the database and to execute queries on the database which led to extracting every information kept in database.

**Vulnerable URL :** *http://localhost/dvwa/vulnerabilities/sqli/*

**Vulnerable Parameter :** *id*

**Payload :** *1 OR 1=1#*

**How to reproduce this vulnerability :**

     1.  Request this URL: http://localhost/dvwa/vulnerabilities/sqli in browser.

     2.  Input the above payload in the 'id' field.

     3.  It will show the information of users stored in database.

**POC :**
    
   ![sql injection medium](https://user-images.githubusercontent.com/36234942/61727869-b2044c00-ad91-11e9-91b1-cef49c7c474a.PNG)
