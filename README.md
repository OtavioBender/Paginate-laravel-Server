# Paginate-laravel-Server
When pagination working fine in localhost but not working on the production, change nginx file. 
GET method doesn't bring the parameters correctly.

ALTER LINE ON FILE: 
try_files $uri $uri/ /index.php;

TO:
try_files $uri $uri/ /index.php?$query_string;

