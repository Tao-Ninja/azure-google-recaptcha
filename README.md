# azure-google-recaptcha
Google Recaptcha v3 built on an Azure Function with C#

URL: http://localhost:7071/api/isHuman 
Method: POST
Body: JSON
{
“token”:”here token by google” 
}
Responses:
200 OK: With message “Human”, Only when user is human. 200 will be in only one case which is this one.
400 BadRequest: With message “Not Human”
400 BadRequest: If api fails or body is not passed will be given a response
with appropraite message
