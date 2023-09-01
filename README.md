# Linkding
Linkding is a self-hosted bookmark manager.

The original repo is https://github.com/sissbruecker/linkding

## Installation
1. Create VM/Container with docker
2. Create two files: .env and docker-compose.yml in the destination folder
3. Run from the folder
   ```
   docker-compose up -d
   ```
4. For security reasons, the linkding Docker image does not provide an initial user, so you have to create one after setting up an installation. To do so, replace the credentials in the following command and run it:
   ```
   docker-compose exec linkding python manage.py createsuperuser --username=joe --email=joe@example.com
   ```
