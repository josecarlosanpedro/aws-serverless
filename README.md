# aws-serverless

sample serverless function with API gateway with AWS

## How to use
1. git clone https://github.com/josecarlosanpedro/aws-serverless.git
2. yarn install/npm install
3. serverless deploy (For more info go to [Serverless](https://www.serverless.com))

## For Serverless offline 
1. git checkout serverless-offline
2. yarn install/npm install
3. serverless deploy (For more info go to [Serverless](https://www.serverless.com))

### To Test serverless offline
POST
curl -X POST http://localhost:3000/dev/todos --data '{ "text": "Learn Serverless" }'
PUT
curl -X PUT http://localhost:3000/dev/todos/<id> --data '{ "text": "Update Serverless" }'
DELETE
curl -X PUT http://localhost:3000/dev/todos/<id>
GET
curl -X GET http://localhost:3000/dev/todos/<id>
GET LIST
curl -X GET http://localhost:3000/dev/todos
