Generalised Mail Transport Protocol 

The core SMTP protocol is ammended as follows:

1/ Relay agents identify themselves with a GPG fingerprint instead of a hostname;
2/ Authenticating username is the identity associated with the key to protect against namespace colisions;
3/ Password is the identity associated with the the other key
4/ The sending relay signs the DATA payload 

Will probably joggle that around a bit and begin work on a proof of concept.
