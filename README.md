# Vuln-AdminLTE-3.2.0

Vendor Homepage: https://adminlte.io/ Software 
Link: https://github.com/ColorlibHQ/AdminLTE/releases/tag/v3.2.0 
Version: 3.2.0 
Tested on: tuition.staging-rdegi.com
CVE:
Author Github: github.com/SHN011
Instagram:@kabil__esh
Description :
This submission details an authentication bypass and privilege escalation vulnerability in AdminLTE 3.2.0. By exploiting a specific sequence of actions involving local account creation and URL manipulation, an attacker can gain unauthorized access to the administrative panel. Proof of Concept   
Navigate to the AdminLTE 3.2.0 instance: https://tuition.staging-rdegi.com/website/AdminLTE-3.2.0/index.php   
 Create a new local user account with a fake email and user credentials.    
 Attempt to log in to the admin panel using incorrect credentials. After the login attempt fails and the system redirects to admin_login.php, observe the "user and password wrong" message.after In the browser's address bar, replace /admin_login.php or /login.php with index.php. The system will bypass the login and redirect to the administrative panel.  Impact Successful exploitation of this vulnerability allows unauthorized users to bypass the authentication mechanism and gain access to the administrative panel. This could lead to a compromise of the application and potentially the underlying server, depending on the privileges of the AdminLTE instance.
