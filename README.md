**Docker Setup for Ruby on Rails with PostgreSQL**

Here's a step-by-step guide to create a Dockerized Ruby on Rails application with PostgreSQL running in a separate container.

Step 1: Create a new Rails application (if you don't have one)
First, let's create a simple Rails app configured for PostgreSQL:

bash
# Create a new Rails app with PostgreSQL as database
rails new myapp --database=postgresql
cd myapp

Step 2: Create the Dockerfile

Step 3: Create an entrypoint script
bash
chmod +x entrypoint.sh

Step 4: Create a docker-compose.yml file

Step 5: Configure database.yml

Step 6: Build and run the application
Run the following commands:

bash
# Build the images
docker-compose build

# Create the database
docker-compose run web rails db:create

# Run the application
docker-compose up

Step 7: Access the application
Your Rails application will be available at http://localhost:3000
