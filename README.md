# docker-nginx-proxy-le

## Run the service stack
`docker-compose up`

## Request the cert of the first time
`docker-compose run --rm certbot certonly --webroot --webroot-path /var/www/certbot/ -d [domain-name]`

## Cron renewal
`docker-compose run --rm certbot renew`

## Setup any proxies etc here AND the SSL config lines
`$EDITOR nginx/conf/nginx.conf`
