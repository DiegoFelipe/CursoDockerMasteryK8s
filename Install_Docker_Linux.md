# Installing Docker on Linux

## Curl Method

- Install the Edge version
- RHEL only supports Docker EE
- Amazon Linux doesn't support Docker
  
*curl -fsSl get.docker.com -o get-docker.sk*

## Install Docker Machine

base=https://github.com/docker/machine/releases/download/v0.16.0 &&
>   curl -L $base/docker-machine-$(uname -s)-$(uname -m) >/tmp/docker-machine &&
>   sudo mv /tmp/docker-machine /usr/local/bin/docker-machine &&
>   chmod +x /usr/local/bin/docker-machine

## Install Docker compose

- sudo curl -L "https://github.com/docker/compose/releases/download/1.25.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
- sudo chmod +x /usr/local/bin/docker-compose
  

## Important Notes

- Every 2 months, update docker machine and docker compose.
