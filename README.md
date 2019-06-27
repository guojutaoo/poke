# README

## Getting started

Install Docker


```bash
# Build the rails app
docker-compose build

# Start the rails app
docker-compose up -d

# Verify `postgres` and `web` (rails) are running
docker-compose ps

# Visit localhost:3000, you will see a page saying the databases are not yet created

# Create the databases
docker-compose run web rake db:create

# Visit localhost:3000, it should work

```
