```
host :dev.pango-apis.com
scheme : http
baseUrl: /apis/v1
```
Sample Request/response
`POST http://dev.pango-apis.com/apis/v1/authenticate`
request headers `Content-Type →application/json` and `Accept →application/json`
---RequestBody
```
{
	"userName": "iddy.magohe@ceitechs.com",
	"password": "123456"
}
```
-- ResponseBody 
```
{
  "firstName": "Iddy",
  "lastName": "Magohe",
  "userReferenceId": "584f69d8e4b00407a1afd4d5",
  "user-token": "iddy.magohe@ceitechs.com:1481603354762:7eff8d25128eb89611e4c058d85c23ca"
}
```
for most of the api calls you'll need the `user-token` (store it in a secure cookie), tokens expires after 60mins, so the user should login agin
for now use the above user details, first & lastname is for  UI presentment 