# Web Stack Boilerplate

## How to use

1. Clone this repo
2. Copy and rename _.env.dist_ file to _.env_. If you need you can change some settings there.
3. Add to your system _hosts_ file domain from _.env_ (option _APP_HOST_). We don't recommend to use _localhost_.
4. Build docker images  
   Run this command from project root folder:
   ```
   $ docker-compose build
   ```
5. Run docker stack
   ```
   $ docker-compose up -d
   ```
6. Add your application to _/src/_ folder.
7. If you need you can use Composer from container like:
   ```
   $ docker-compose exec phpfpm composer install -a
   ```