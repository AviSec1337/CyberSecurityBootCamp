## Install Docker on Ubuntu

```bash
# Update package list
sudo apt update

# Install required packages
sudo apt install -y ca-certificates curl gnupg lsb-release

# Create directory for Docker's GPG key
sudo mkdir -p /etc/apt/keyrings

# Add Docker's official GPG key
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

# Set up the Docker stable repository
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] \
https://download.docker.com/linux/ubuntu \
$(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Update package list again to include Docker packages
sudo apt update

# Install Docker Engine, CLI, containerd, Buildx, and Compose plugin
sudo apt install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
