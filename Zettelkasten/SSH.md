202407222243

Status: #permanent

Tags: [[20240724-Remote-Server-Administration]] [[20240724-Network-Security]] [[Born2beRoot]]
#ssh #networking #security #remote-access

# SSH (Secure Shell) 
## Key Features of SSH 
- **Encryption**: Ensures data transmitted between client and server is secure. 
- **Authentication**: Verifies identities using passwords, public key authentication, etc. 
- **Data Integrity**: Ensures data is not altered during transmission. 
- **Port Forwarding/Tunneling**: Secures otherwise insecure protocols. 
- **Secure File Transfer**: Uses SCP and SFTP protocols for secure file transfer. 
## How SSH Works 

1. **Connection Establishment** 
	- Client initiates connection. 
	- Server responds with public key; session key established. 
2. **Authentication** 
	- Client authenticates (e.g., password, public key). 
	- Public key authentication: public key on server, client uses private key. 

3. **Data Transmission** 
- Secure exchange of data post-authentication. 
- Commands issued by client executed on server. 

## Common Uses of SSH 
- **Remote Login**: Secure administration of remote servers. 
- **Remote Command Execution**: Running commands on remote machines. 
- **Secure File Transfers**: SCP or SFTP for secure file movement. 
- **Port Forwarding**: Securing connections through tunneling. 
## Advantages of SSH

- **Security**: Strong encryption and authentication methods.
- **Versatility**: Applicable for various tasks.
- **Widely Supported**: Available on most OS and network devices.


## Example of Using SSH 
```sh 
ssh username@remote_server_ip
```
With public key authentication:
```sh 
ssh -i /path/to/private_key username@remote_server_ip
```

---
#References

1. https://de.wikipedia.org/wiki/Secure_Shell