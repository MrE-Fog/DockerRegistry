# docker-registry

## How to setup

# Authentication
apt install apache2-utils
htpasswd -c password admin
cp password nginx/auth

# Get SSL Certificate
[SSLforFree](htttp://sslforfree.com)
cat sertificate.crt ca_bundle.crt > server.crt
cp private.key certs
cp server.crt certs

# Launch
> docker-compose up
