# General Mail Transport Protocol 

## Working draft

The core SMTP protocol is ammended as follows:

S: 220 <fingerprint> General Mail Transfer Service Ready

C: EHLO postmaster@client.example.com

S: 250-smtp.server.com Hello postmaster@client.example.com

S: 250-SIZE 1000000

S: 250 AUTH LOGIN

C: AUTH PLAIN

S: 334 VXNlcm5hbWU6

C: <base64 postmaster@server.example.com>

S: 334 UGFzc3dvcmQ6

C: <base64 fingerprint for postmaster@client.example.com>

S: 235 2.7.0 Authentication successful
 
## Reference 

1. [SMTP/ESMTP](https://www.samlogic.net/articles/smtp-commands-reference.htm)
2. [AUTH mechanisms](https://www.samlogic.net/articles/smtp-commands-reference-auth.htm)
