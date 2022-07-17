# Start Project
1. After creating Dockerfile, run the following command:
***docker-compose run app rails new . --force --database=mysql --skip-bundle***

    This command will create a Rail structure project and it will update some
    files. Since previous command will create project as root, probably,
    it would be necessary to run:

      ***sudo chown -hR {user}:{user} .***

2. Then, and before running *make up* command, please install *rails webpacker* with the following command:
***docker-compose run app rails webpacker:install***

3. Finally, run ***make up*** command.

# References
1. https://dev.to/itnext/setting-up-ruby-on-rails-with-docker-and-mysql-3mpc
