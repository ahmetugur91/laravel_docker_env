# LARAVEL DOCKER

## INSTALL
- Put your laravel project in this directory `as a folder`
- Go to your laravel folder `cd yourfolder`
- Composer install
    - On Linux/MacOS: `docker run --rm -v $(pwd):/app composer install`
    - On Windows in PowerShell: `docker run --rm -v ${PWD}:/app composer install`
    - On Windows in CMD: `docker run --rm -v %cd%:/app composer install`
- Create .env file `cp .env.example .env` 
- Go back to root folder `cd ..`
- Start docker compose `docker-compose up`
- Go to your laravel folder again `cd yourfolder`
- Generate key for laravel app `docker-compose exec app php artisan key:generate`