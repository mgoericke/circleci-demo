# circleci-demo
Deploy serverless project with CircleCI


## Create a new nodejs project:

```
$ mkdir circleci-demo
$ npm init
```

## Install Serverless Framework

```
$ npm i -D serverless serverless-offline
```

## Install testing dependency (jest)
```
$ npm i -D jest
```
create test (handler.test.js) and add test command to package.json

```
"scripts": {
  "test": "jest"
}
```

## Create handler.js and fill with code

`@see code`

## Run locally
Create a serve command to run the service locally with `serverlerss-offline` plugin

```
"script": {
  "serve": "serverless offline start",
  ...
}
```

# Automating deployments with CircleCI
Setup a CircleCI account (with github). Add AWS credentials (create  IAM credentials)

### Add CircleCI config
```
$ mkdir .circleci
$ touch config.yml
```

`@see code`
