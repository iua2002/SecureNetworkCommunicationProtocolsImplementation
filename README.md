Network Security Project:
This project involves implementing a secure Diffie-Hellman key exchange protocol and developing SSL/TLS-enabled web client and server using Python. The project ensures secure communication between client and server using both self-signed and Let's Encrypt certificates. Additionally, network traffic analysis with and without SSL is performed to demonstrate the differences in secure and encrypted data transmission.

Files:
diffie_hellman_client.py: Implements the client side of the Diffie-Hellman key exchange protocol.
diffie_hellman_server.py: Implements the server side of the Diffie-Hellman key exchange protocol.
ssl_web_client.py: Implements an SSL/TLS-enabled web client.
ssl_web_server.py: Implements an SSL/TLS-enabled web server.

Requirements:
Python 3.x
ssl library
socket library
mypy (optional, for type checking)
certbot (for obtaining Let's Encrypt certificates)

Installation
Clone the repository:
  git clone https://github.com/yourusername/network-security-project.git
  cd network-security-project
  
Install Python and dependencies:
  sudo apt-get update
  sudo apt-get install python3 python3-pip
  pip3 install --upgrade mypy
  
Install Certbot:
Follow the instructions for your environment from Certbot's official site.

Usage
Diffie-Hellman Key Exchange
Run the server:
  Copy code
  python3 diffie_hellman_server.py

Run the client:
  python3 diffie_hellman_client.py
  SSL/TLS Web Client and Server
  
Run the server without SSL:
  python3 ssl_web_server.py --address 0.0.0.0 --port 8000
  
Run the server with SSL:
  python3 ssl_web_server.py --address 0.0.0.0 --port 443 --ssl --cert-file <path-to-cert> --key-file <path-to-key>
  
Run the client without SSL:
  python3 ssl_web_client.py www.example.com --port 80
  
Run the client with SSL:
  python3 ssl_web_client.py www.example.com --ssl --port 443
  
Analyzing Network Traffic
Capture packets on port 8000 without SSL:
  sudo tcpdump -i lo -A port 8000
  
Capture packets on port 8000 with SSL:
  sudo tcpdump -i lo -A port 8000
  
Now you can observe the number of packets and the differences between SSL and non-SSL transmissions
