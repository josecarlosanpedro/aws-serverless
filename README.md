# aws-serverless

sample serverless function with API gateway with AWS

## How to use
  ### Setting up severless connection to amazon via terminal
   1. npm install -g serverless
   2. serverless config credentials --provider provider --key key --secret secret
   
        -- [Amazon Security Credential](https://console.aws.amazon.com/iam/home?region=us-east-1#/security_credentials)
        
        -- Go to "Access keys for CLI, SDK, & API access"
        
        -- Click Create Access Key and it will generate your key and secret
  ### Using this project 
   1. git clone https://github.com/josecarlosanpedro/aws-serverless.git
   2. yarn install/npm install
   3. serverless deploy (For more info go to [Serverless](https://www.serverless.com))

## For Serverless offline 
1. git checkout serverless-offline
2. yarn install/npm install
3. sls offline start (For more info go to [Serverless](https://www.serverless.com))

##### To Test serverless offline
    POST: curl -X POST http://localhost:3000/dev/sample --data '{ "text": "Learn Serverless" }'

    PUT: curl -X PUT http://localhost:3000/dev/sample/{id} --data '{ "text": "Update Serverless" }'

    DELETE: curl -X PUT http://localhost:3000/dev/sample/{id}

    GET: curl -X GET http://localhost:3000/dev/sample/{id}

    GET LIST:  curl -X GET http://localhost:3000/dev/sample

## For serverless AWS and DynamoDB

1. git checkout serverless-aws-dynamodb
2. yarn install/npm install
3. serverless deploy (For more info go to [Serverless](https://www.serverless.com))

##### To Test serverless with dynamoDB
    POST: curl -X POST https://XXX.execute-api.us-east-1.amazonaws.com/dev/sample --data '{ "text": "Learn Serverless" }'

    PUT: curl -X PUT https://XXX.execute-api.us-east-1.amazonaws.com/dev/sample/{id} --data '{ "text": "Update Serverless" }'

    DELETE: curl -X PUT https://XXX.execute-api.us-east-1.amazonaws.com/dev/sample/{id}

    GET: curl -X GET https://XXX.execute-api.us-east-1.amazonaws.com/dev/sample/{id}

    GET LIST:  curl -X GET https://XXX.execute-api.us-east-1.amazonaws.com/dev/sample

###### or

Go to [Amazon DynamoDB](https://console.aws.amazon.com/dynamodb/home?region=us-east-1#tables:selected=serverless-carlo-dev;tab=items) to check the items if exists
