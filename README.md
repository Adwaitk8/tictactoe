# Tic-Tac-Toe game in Oracle PL/SQL

### Overview

An sql script that runs a game of tic-tac-toe.

### How to run:

To run the script, open oracle through command prompt in the same
directory as the SQL script.
```sh
$ sqlplus '/ as sysdba'
```

Triggers can't be created on SYS user. Hence, a new user should be
created. Create new user using following commands:


Switch to Pluggable database (ORCLPDB)
```sh
$ alter session set container = ORCLPDB;
```

Create User:
```sh
create user user_name identified by password;
```

Switch user:
```sh
conn user_name/password@localhost:1521/orclpdb
```

Run Script
```sh
@tictactoe
```
