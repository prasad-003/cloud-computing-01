# Cloud Computing Lab Assignment

This repository contains a simple web application hosted on an AWS EC2 instance.

## Project Details
* **College**: Sahyadri College of Engineering and Management
* **Student Name**: Prasad Achari
* **USN**: 4sf23cs150
* **Department**: CSE (Computer Science and Engineering)
* **Section**: 7C

## Live Application Link
* **Public Server IP**: http://16.170.166.57:8080

  
<img width="676" height="891" alt="Screenshot 2026-07-21 144025" src="https://github.com/user-attachments/assets/c66cd5b4-94a7-48cc-82d7-3c30d0efb305" />


# Update the system
sudo yum update -y

# Install Apache
sudo yum install httpd -y

# Start Apache
sudo systemctl start httpd

# Enable Apache at boot
sudo systemctl enable httpd
# OR
sudo systemctl enable --now httpd

# Check Apache status
sudo systemctl status httpd

# Create HTML file
nano index.html

# Copy HTML file to Apache web root
sudo cp index.html /var/www/html/index.html

# Set ownership and permissions
sudo chown apache:apache /var/www/html/index.html
sudo chmod 644 /var/www/html/index.html

# View deployed HTML
cat /var/www/html/index.html

# List files in web root
ls -l /var/www/html

# Restart Apache
sudo systemctl restart httpd

# Stop Apache
sudo systemctl stop httpd

# Start Apache
sudo systemctl start httpd

# Check Apache status
sudo systemctl status httpd

# Get EC2 Public IP
curl ifconfig.me
------------------------------------------------------------------------------------------------------------------------------------------
