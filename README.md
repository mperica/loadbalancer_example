# Example of Loadbalancer and Docker-Compose

Docker technology is an easy way to spin virtual machines for specific tasks.
In this example 3 virtual machines each for its own task:
  -	Website1: Serving apache + PHP and displaying content of the website folder
  -	Website2: Serving apache + PHP and displaying content of the website folder
  - Loadbalancer: Serving Haproxy and balancing traffic from users to Website1 and Website2


## Usage:
Considering you have Docker installed and running.

```
docker-compose up # To run in the terminal for live preview
docker-compose up -d # To run in the background
docker-compose ps # To see running instances
docker-compose down # To stop docker-compose running in the background
```
Now that docker-compose is running got to [localhost](http://localhost) and each time you refresh it will show one of the websites.
