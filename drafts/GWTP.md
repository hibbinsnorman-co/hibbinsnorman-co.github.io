# General Web Transport Protocol 

## Working draft

The core HTTP protocol is ammended as follows:

1. Server signature is clarified to mean a certificate fingerprint
2. Auth challenge to include the server realm per SAML/LDAP
3. Auth user to identify scoped username
4. Auth password to mean fingerprint of user key as known to challenging realm.
5. When an unauthorized response is given the server should include a body with the public key identified by the fingerprint 

## Reference 

1. TODO
