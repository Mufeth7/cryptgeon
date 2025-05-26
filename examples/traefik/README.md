# Install Cryptgeon with Traefik

What is Traefik?

Traefik is a modern, open-source application proxy that acts as a reverse proxy and ingress controller. Here we used to get SSL Certificate using Let's Encrypt.

# How to Setup Traefik to get SSL certificate for your Domain
# Step 1:
Clone  this repository in your Host Machine. 

# Step 2:
# In your Host Machine Create Directory in OPT Directory 
    ```
    cd /opt && mkdir traefik
    ```

# Step 3:
# Create acme.json file in /opt/traefik/ Directory
   
    ```
    touch acme.json
    chmod 600 /opt/traefik/acme.json
    ```
# Step 4:
Then come to the cloned cryptgeon directory use this docker-compose file [Docker-compose file](docker-compose.traefik.yaml) and edit inside the docker-compoose file add your Email on line no:22 and Domain name on line no: 59 

# Step 5:
Let's up the container 
    ```
    docker-compose up -d
    ```