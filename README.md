Network Security Project
This project involves implementing a secure Diffie-Hellman key exchange protocol and developing SSL/TLS-enabled web client and server using Python. The project ensures secure communication between client and server using both self-signed and Let's Encrypt certificates. Additionally, network traffic analysis with and without SSL is performed to demonstrate the differences in secure and encrypted data transmission.

Files
diffie_hellman_client.py: Implements the client side of the Diffie-Hellman key exchange protocol.
diffie_hellman_server.py: Implements the server side of the Diffie-Hellman key exchange protocol.
ssl_web_client.py: Implements an SSL/TLS-enabled web client.
ssl_web_server.py: Implements an SSL/TLS-enabled web server.

Requirements
Python 3.x
ssl library
socket library
mypy (optional, for type checking)
certbot (for obtaining Let's Encrypt certificates)
