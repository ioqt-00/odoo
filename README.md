# Requirements

You need docker & docker-compose installed to run this.
On Debian, you can install them running:

sudo apt-get install docker
sudo apt-get install docker-compose

# Launch stack

export DB_PASSWORD=replace_with_your_database_password; docker-compose -f docker-compose.yml up

This will download postgre & odoo docker images, install them and run them with the parameters define on docker-compose

Then, visit http://localhost:8069 using a browser.

# Information
This repo contains a docker compose file, the accounting module Odoo 15 Accounting from the odoomates GitHub repo, and a few config files. The docker compose file will run an odoo instance on port 8069, with the Accounting module in the right folder, and give an easy way to configure the odoo instance.

Note that once you have installed the odoo instance, you can delete unavailable apps in the "Apps" menu, using the "List" layout (button on top right)
