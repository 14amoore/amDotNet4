# This dockerfile is used for local development. Installs extra postgres packages, like pg_cron.
FROM postgres:14.5
RUN apt-get update && apt-get -y install postgresql-14-cron && rm -rf /var/lib/apt/lists/*
ARG POSTGRES_USER=root POSTGRES_PASSWORD=root
