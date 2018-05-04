How to prepare MySQL for the Demo
============================================

## Install Tools

1. Install unzip and git with `apt-get install unzip git wget`


## Clone repo

2. Clone this repo: `git clone https://github.com/puckpuck/planespotter.git`
3. Change the two DB shell scripts to be executable `chmod +x ./planespotter/db-install/*.sh`


## Create Database

4. Execute the DB creation script `./planespotter/db-install/create-planespotter-db.sh`. 
NOTE: The password that gets asked, is the MySQL Root Password.


## Cleanup

If you ever want to recreate the database, you can use the DB deletion scrip `./planespotter/db-install/delete-planespotter-db.sh` to drop the DB, and then Create the Database again.

