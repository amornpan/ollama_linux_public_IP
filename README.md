# ollama_linux_public_IP

```
Open the ollama.service file with a text editor:

sudo vi /etc/systemd/system/ollama.service

Add the following line under the [Service] section:
new line !!

[Service]
Environment="OLLAMA_HOST=0.0.0.0:11434"

```
![alt text](https://images.cloudclusters.io/7d7a0864c27746d2b5ed32b8dffc8880/EditOllama.service.jpg)

```
Restart the Service - After modifying the service file, reload the systemd configuration and restart Ollama:

sudo systemctl daemon-reload
sudo systemctl restart ollama
3. Access and Test - Once Ollama has been restarted, it will be accessible via the public IP address. Ensure your network and firewall settings permit external access.
```
![alt text](https://github.com/user-attachments/assets/3a9d0312-298d-4618-a7da-e7fb23586c2e)

