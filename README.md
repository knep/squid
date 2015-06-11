# squid
Based ubuntu-debootstrap:latest  
Simple proxy with basic authentication.  
[apache2-utils required] to create the file for the authentication:  
**htpasswd -c /local_path/passwd_file user** 

Launch command:  
**docker run -d -p 3128:3128 -v /path/to/passwd_file:/etc/squid/passwd --name proxy knepti/squid**
