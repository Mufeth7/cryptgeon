# Install Cryptgeon with Traefik

What is Traefik?
Traefik is a modern, open-source application proxy that acts as a reverse proxy and ingress controller. Here we used to get SSL Certificate using Let's Encrypt.

# How to Setup Traefik to get SSL certificate for your Domain
# Step 1:
Clone  this repository in your Host Machine. 

# Step 2:
# In your Host Machine Create Directory in OPT Directory 
    ```sh
  # create this directory in your Hosting instance.
    cd /opt && mkdir traefik
    ```

# Step 3:
# Create acme.json file in /opt/traefik/ Directory
   
    ```sh
    touch acme.json
   
   #  Give permission to this acme.json file
    chmod 600 /opt/traefik/acme.json
    ```
# Step 4:
# Then use this compose file [Docker-compose file](examples/traefik/docker-compose.traefik.yaml)