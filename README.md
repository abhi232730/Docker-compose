# Docker-compose
Run two Nginx docker containers in active-passive mode by using Keepalived.
The containers must be based on an Ubuntu 16:04 image.
The goal is to ensure one Nginx service is running at all times.
Nginx containers should be called keepalived_master/keepalived_backup.
Both containers should contain
• keepalived installed and configured
• nginx with a simple web page (hello I’m master/backup!).
• Master’s Nginx webpage is served on port 8880 to the host machine.
• Slave’s Nginx webpage is served on port 8881 to the host machine.
To run everything use docker-compose up
