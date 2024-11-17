# coding-project-template

Test the /register and /login with cURL commands for the following cases. Make a note of the response messages on notepad or any other editor.
Register with a new username, password, email:

curl  -X POST  -H 'Content-Type: application/json'  -d '{
    "username":"coopercoote",
    "email":"ccoote@gmail.com",
    "password":"cg123"}' -k 'http://localhost:3000/register'

----------------------------------------------------------------
Login with username password you just registered:

curl  -X POST  -H 'Content-Type: application/json'  -d '{
    "username":"coopercoote",
    "password":""}' -k 'http://localhost:3000/login'