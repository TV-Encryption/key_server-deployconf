# key_server Deployconf

Quick and dirty deployment configuration.

## How to use

1. Clone `key_server` project in this projects directory.
2. Run the following command to get a Djano secret key:
   ```shell
   docker run --rm django python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())"
   ```
3. Copy `.env.example`to `.env` and fill out all empty settings.
4. `docker-compose up -d`