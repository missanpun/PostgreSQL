# PostgreSQL
This guide walks you through downloading, installing, and connecting to a PostgreSQL database on Windows, macOS, and Linux (Ubuntu/Debian) systems.

#Download & Install PostgreSQL for windows
Go to: https://www.postgresql.org/download/windows/

Download the installer (from EDB).

Run the installer:

Choose default components.

Set a password for the postgres superuser.

Note the port (default: 5432).

Installation also includes pgAdmin (a GUI tool).


# macOS (via Homebrew)
Open Terminal.
Run the following commands:

brew update
brew install postgresql
brew services start postgresql
# check the version.
psql --version

# You can access the window from cmd mode.
1. copy this path 
C:\Program Files\PostgreSQL\15\bin
2. Add it to the PAth:
   .Press win + s -Search "Environment Variables"
   .Click "Edit the sytem enviroment variable"
   .in Sytem Properties, click Environment Variale
   .in system variable, find and select the path -click edit
   .click new and past:
   C:\Program Files\PostgreSQL\15\bin
.Click OK to close all dialogs.
3. Reopen commad promt and test:
 psql --version

.You should see somting like:
psql (PostgreSQL) 15.x

# For SQL connection write a command
 sql -U postgres
 .Give your password (you are setting psswod during installation) 
 Password for user postgres:
.After you shoud see like:
postgres=# 
