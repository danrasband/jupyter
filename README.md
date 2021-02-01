# Jupyter Lab via docker-compose

This repo allows you to use Jupyter Lab via docker-compose:

```bash
docker-compose up jupyter
```

It also has Postgres in case you need it. Additional services can
be added in the future.

The docker-compose setup assumes you use the following folders for your
data and projects:

```bash
$HOME/Data/
$HOME/Projects/
```

If you use a different setup, then feel free to fork this repo and adjust the
appropriate lines in docker-compose.yml.
