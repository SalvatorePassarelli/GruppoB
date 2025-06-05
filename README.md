
# 🚀 WebUI LLM Deployment with Docker 🧠🐳
Welcome to our repository! Inside, you'll find everything you need to launch a powerful WebUI preloaded with a Large Language Model (LLM) — all made seamless and effortless with Docker and Docker Compose. 🌐✨

# 📦 What is this project?
This repository provides a fully configured setup to:

📁 Run a custom Dockerfile tailored for building the required environment

🔧 Use a docker-compose.yml file to launch the application with a single command

🧠 Load and serve a pre-installed LLM (Large Language Model)

💻 Offer a clean and interactive WebUI for engaging with the model

Our mission is to deliver a plug-and-play tool for developers, researchers, or enthusiasts who want to interact with LLMs without dealing with complex environments or dependencies.

# 🚀 Getting Started
## 1. Clone the repository

bash
<pre> git clone https://github.com/SalvatorePassarelli/GruppoB </pre>
cd your-repo
## 2. Launch the environment
bash
<pre> docker-compose up -d </pre>
⏳ Wait a few moments while Docker builds the image and starts the services. Once ready, open your browser and go to:

## 3. Configure DNS and Domain:

Log in to your domain provider (e.g., DuckDNS) and create a domain.
Point the domain to your proxy’s local IP (e.g., 192.168.0.6).
If using DuckDNS, get an API token from their dashboard.
Here is a simple example how it's done in https://www.duckdns.org/domains :
Set Up SSL Certificates:
Access Nginx Proxy Manager at http://server_ip:81. For example: 192.168.0.6:81
Log in with the default credentials (admin@example.com / changeme). Change them as asked.
Go to SSL Certificates → Add SSL Certificate → Let's Encrypt.
Write your email and domain name you got from DuckDNS. One domain name contains an asterisk and another does not. Example: *.hello.duckdns.org and hello.duckdns.org.
Select Use a DNS challenge, choose DuckDNS, and paste your API token. example: dns_duckdns_token=f4e2a1b9-c78d-e593-b0d7-67f2e1c9a5b8
Agree to Let’s Encrypt terms and save. Change propagation time if needed (120 seconds).
Create Proxy Hosts:
For each service (e.g., openwebui, nextcloud), go to Hosts → Proxy Hosts → Add Proxy Host.
Fill in the domain name (e.g., openwebui.hello.duckdns.org).
Set the scheme to HTTP (default), enable Websockets support and point to your Docker IP (if docker with open-webui is running on the same computer as NGINX manager, this will be the same IP as earlier (example: 192.168.0.6)
Select the SSL certificate generated earlier, force SSL, and enable HTTP/2.

browser
<pre> http://localhost </pre>
✨ Key Features
✅ Automated and transparent setup

🧠 Integrated with a powerful LLM

🖥️ Simple, elegant, and responsive WebUI

🔄 Easily customizable for a wide range of use cases




# 📚 Requirements
Docker (v20+ recommended)
Docker Compose
Internet connection for initial model download

# 🤝 Contributing🛠️
Project developed in collaboration with:
# 🧑‍💻Students of CyberHackademy
# 📬 Contact
🧑‍💻https://github.com/ldcostanzo
🧑‍💻https://github.com/giovannids100
🧑‍💻https://github.com/MattiaScotti/
A collective effort combining learning, creativity, and cutting-edge tech. 🚀



