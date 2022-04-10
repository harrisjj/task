# task
PHP Code Challenge
Step 1:
composer update
Step 2:
Create database projectapi in phpmyadmin
.env file add db name and password

Step 3:
Run command php artisan migrate

Set Employee data:

php artisan empdata:SET 1 test 191.78.1.1

Get Employee data:

php artisan empdata:GET 191.78.1.1

Output : [{"emp_id":1,"emp_name":"test","ip_address":"191.78.1.1"}]

Unset Employee data:

php artisan empdata:UNSET 191.78.1.1


Set Employee Web History data:

php artisan empwebhistory:SET 191.78.1.1 https://google.com

Get Employee Web History data:

php artisan empwebhistory:GET 191.78.1.1

Output : {"emp_id":2,"ip_address":"191.78.1.2","urls":[{"url":"https:\/\/google.com","id":2},{"url":"https:\/\/google.com","id":3}]}

Unset Employee Web History data:

php artisan empwebhistory:UNSET 191.78.1.1
