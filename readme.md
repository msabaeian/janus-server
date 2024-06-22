## Install docker and docker compose
https://docs.docker.com/engine/install/ubuntu/

https://docs.docker.com/compose/install/linux/


## Start Janus
copy `docker-compose.yml` and `/conf` somewhere and run: 
`sudo docker compose up`

Note: remember to change your configs


## Config ngnix
`sudo vim /etc/nginx/sites-available/default`

paste content of nginx.conf, repalce SERVER_IP (in two places) with your server IP, modify ssl_certificate with your own data, save and reload nginx:

`sudo systemctl reload nginx`
