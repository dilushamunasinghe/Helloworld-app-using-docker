# pull image 
FROM postgres

# Set the environment variable for password to 'docker'
ENV POSTGRES_PASSWORD docker

#Create a database
ENV POSTGRES_DB world

# Using a sql dump file to create the table schema and populate it with data
COPY world.sql /docker-entrypoint-initdb.d/