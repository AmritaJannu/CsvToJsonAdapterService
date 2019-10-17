# CsvToJsonAdapterService
Bulk CSV to JSON data importer service

This Service helps to convert Any CSV Data to JSON.
Output of this Application
1) Outputs the CSV file to sample_users_successfull.json file thats saved into public/downloads folder
2) Outputs the Errorneous Data to sample_users_errors.json file thats saved into public/downloads folder

Technology Used:
PHP 7 
Laravel

How to run it on CLI ?

RUN >php artisan csv2json 

The output should look like this :
For Exqample : 

C:\xampp\htdocs\bigtincan>php artisan csv2json

Count of Successful rows:10
Successful file path: public/downloads/sample_users_successful.json

Count of Error rows:3
Error file path:public/downloads/sample_users_errors.json

Rows which had error
-----------------------------------------------------------
[{"first_name":"","last_name":"","email":"nouser@gmail.com","platforms":["web","ios"],"password":"password","job_title":"","department":""},{"first_name":"Ron","last_name":"Jones","email":"ronjonesatgmail.com","platforms":["web"],"password":"Password3","job_title":"Manager","department":"Management"},{"first_name":"Newt","last_name":"Rick","email":"newt.rick@gmail.com","platforms":["web","ios"],"password":"bad","job_title":"","department":"HR"}]

Files :
Path\app\Http\Services\CsvAdapterService.php
Path\routes\console.php
Path\routes\web.php
Path\app\Http\Controllers\CsvToJsonController.php


The only thing thats missed out is the PHP Unit test due to lack of time.









