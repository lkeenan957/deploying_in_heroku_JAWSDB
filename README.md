# deploying_in_heroku_JAWSDB

Steps:
1. Sign Up for Heroku
2. Find a project which has the complete MVC model with a config file.
3. Go to the project folder in terminal and type : heroku create
4. And go to heroku and click the spcefic project - go to the resources tab 
5. on the add-on section- write JawsDB MySQL
6 . Install it
7. then under add-ons - you will see the JawsDB MySQL appears. 
8. Click on it to get a new page with username, password, host,...
9. Go to your config file: change the username, password, host, check the dialect,
and the production tab:
EXAMPLE:

{
  "development": {
    "username": "s9yg6g72pv2b07um",
    "password": "nwuzkaxd711vimtw",
    "database": "burgers_db",
    "host": "otwsl2e23jrxcqvx.cbetxkdyhwsb.us-east-1.rds.amazonaws.com",
    "dialect": "mysql",
    "port": "3306"

  },
  "test": {
    "username": "root",
    "password": "",
    "database": "database_test",
    "host": "127.0.0.1",
    "dialect": "mysql"
  },
  "production": {
    "use_env_variable": "JAWSDB_URL",
    "dialect":"mysql"
  }
}

10. THen save everything.
11. Then do the steps to push it to git.
  - git add .
  - git commit -m"done"
  - git push origin master
  
12. then type: git push heroku master
13. Then go to heroku and click on the project.
14. It would have deployed!

Hope this file is clear!!!
