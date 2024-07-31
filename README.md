# Update package index
sudo apt update

# Install Python, pip, and virtual environment tools
sudo apt install -y python3 python3-pip python3-venv

# Create and activate a virtual environment
python3 -m venv myenv
source myenv/bin/activate

# Install Ansible, boto3, and botocore with specific versions
pip install ansible>=2.15 boto3>=1.26 botocore>=1.29

# Verify the installations
ansible --version
pip show boto3
pip show botocore
