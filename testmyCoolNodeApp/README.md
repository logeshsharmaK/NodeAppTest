
## Installation

`npm install`


## Run

Run locally:

`DEBUG=custom-idp-starter-kit:* npm start`

Run on the server (use Nginx as a revers proxy):

`pm2 start ./bin/www`

## Testing

Request (both GET & POST are supported):

`curl -d "token=aUserAccessToken" -X POST http://localhost:3000/user/verify`

`curl -X GET http://localhost:3000/user/verify?token=aUserAccessToken`

Response:

`{"uid": xxxxxx}`
