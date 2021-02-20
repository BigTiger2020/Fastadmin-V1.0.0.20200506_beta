# Fastadmin-V1.0.0.20200506_beta - Stored cross-site scripting attacks   
# CVE ID：CVE-2020-22609  
# Affected products：Fastadmin  
# Vulnerability type：Stored cross-site scripting attacks
# Version :V1.0.0.20200506_beta  
# Product manual ：FastAdmin is an extremely fast background development framework based on ThinkPHP5+Bootstrap.  
# Vulnerability description：fastadmin V1.0.0.20200506_beta contains a cross-site scripting (XSS) vulnerability which may allow an attacker to obtain administrator credentials to log in to the background.
1. Through audit analysis of \application\admin\controller\Category.php, it was found that no comprehensive filtering was performed  
![image](https://github.com/BigTiger2020/Fastadmin-V1.0.0.20200506_beta/blob/main/1.png)  
2. Click the category management-edit-nickname box to insert xss statement  
![image](https://github.com/BigTiger2020/Fastadmin-V1.0.0.20200506_beta/blob/main/2.png)   
![image](https://github.com/BigTiger2020/Fastadmin-V1.0.0.20200506_beta/blob/main/4.png)   
3. Rebound administrator identity information  
![image](https://github.com/BigTiger2020/Fastadmin-V1.0.0.20200506_beta/blob/main/5.png)  
4. payload:  
![image](https://github.com/BigTiger2020/Fastadmin-V1.0.0.20200506_beta/blob/main/6.png)  
