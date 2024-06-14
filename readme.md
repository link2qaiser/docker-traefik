To generate a username and password for basic authentication in Traefik, you need to create a hashed password. This can be done using various tools or command-line utilities. One common way is to use the htpasswd command-line utility, which is part of the apache2-utils package

1. Install htpasswd Utility (if not already installed):

```
sudo apt-get update
sudo apt-get install apache2-utils
```

2. Genrate the Credentials

```
htpasswd -nbB user password
```

3. Replace the username credentials and run `docker compose up -d`
