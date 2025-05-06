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


