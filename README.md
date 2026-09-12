Requirements
-----------

  - [Docker](https://www.docker.com)
    - [Docker Compose](https://docs.docker.com/compose/)
  - [GNU Make](https://www.gnu.org/software/make/) (optional)

Installation
------------

  1. Clone the repository

         git clone https://github.com/PHLAK/discord-bot-compose.git

  2. Initialize the configuration files

          make init

     or manually run the commands in `Makefile`

  3. Set the environment variables in `.env`

  4. Set the environment variables in `environment.d/discord-bot.env`

  5. Run `docker compose config` to validate and confirm your configuration

  6. Run `docker compose up -d` to start the containers

  7. Run database migrations

         docker compose exec app php artisan migrate --force