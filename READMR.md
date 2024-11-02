## NGNIX

To run NGINX with WSL (Windows Subsystem for Linux), you’ll need to install WSL, set up an appropriate Linux distribution, install NGINX, and start the server. Here’s the step-by-step process:

# Step 1: Install WSL (if not already installed)
1. Open PowerShell as Administrator and enable WSL:

```bash
wsl --install
```

# Step 2: Update and Install NGINX in WSL
1. Update the package list in your Linux distribution (assuming Ubuntu here):
```bash
sudo apt update
```
2. Install NGINX:
```bash
sudo apt install nginx -y
```
3. Verify Installation by checking the NGINX version:
```bash
nginx -v
```

# Step 3: Start NGINX
1. Start the NGINX service:

```bash
sudo service nginx start
```
2. To check if NGINX is running, use:

```bash
sudo service nginx status
```

# Step 5: Access NGINX from Windows:
```bash
http://localhost
```

# Step 5: Manage NGINX in WSL:
1. Stop NGINX:

```bash
sudo service nginx stop
```
2. Restart NGINX:

```bash
sudo service nginx restart
```
3. Reload NGINX (to apply changes without a full restart):

```bash
sudo service nginx reload
```
