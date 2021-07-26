# PostgreSQL Cheat Sheet

- To remove postgresql: 
  - ```dpkg -l | grep postgres```
  - ```sudo apt-get --purge remove (all the package)```
  - ```sudo rm -rf /var/lib/postgresql/ && sudo rm -rf /var/log/postgresql/ && sudo rm -rf /etc/postgresql/```

- To install postgresql: 
  - ```sudo apt-get install postgresql```

- To change default postgres password:
  - ```sudo -u postgres psql```
  - ```ALTER USER postgres PASSWORD '(some_password)';```

- To connect to postgresql shell:
  - ```psql -U (username) -h localhost```
  - List all existing user: ```\du```

- Create new user:
  - ```CREATE USER (username) WITH CREATEDB LOGIN ENCRYPTED PASSWORD '(password)';```

- Grant database privileges to a user:
  - ```GRANT ALL PRIVILEGES ON DATABASE (databaseName) TO (username);```



### **Currnet postgres user password: root**
