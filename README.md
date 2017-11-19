## You Tube Clone 

### Instructions
- `git clone https://github.com/benjaminadk/youtube-clone.git`
- `cd youtube-clone`
- `npm install`
- `cd client`
- `npm install`
- create `client/config/dev.js`
- add your personal keys

### A Full Stack React App Tutorial Series

#### Video 1 - Intro
- initialize project and install express, babel, etc

#### Video 2 - Graphql Basics
- endpoints, graphql, graphiql, schema, resolvers

#### Video 3 - Graphiql
- setup graphiql GUI

#### Video 4 - Mlab
- setup mlab and mongoose

#### Video 5 - User model
- basic user model

#### Video 6 - Passport 
- finish models install passport

#### Video 7 - Passport 2
- create a google app

#### Video 8 - Passport 3
- test it out and summary of google oauth20

#### Video 9 - Saving a User
- mongoose basics

#### Video 10 - Refactor Schema
- align with mongoose values
- install concurrently and create react app

#### Video 11 - Material UI
- install latest material ui and apollo 

#### Video 12 - React Router
- basic setup 

#### Video 13 - Apollo Frontend Test
- first apollo react component

#### Video 14 - Bug Fixes
- cors, typos, npm packages

#### Video 15 - Navigation
- material ui appbar and drawer

#### Video 16 - Navigation Icons
- link to upload, classes

#### Video 17 - Upload Component
- component style and layout
- use resource upload background

#### Video 18 Video Model
- create video model on backend

#### Video 19 Json Web Token
- create a json web token on login

#### Video 20 Json Web Token 2
- fetching jwt on frontend

#### Video 21 Json Web Token 3
- finalize jwt fetching

#### Video 22 Json Web Token 4
- transfer jwt to backend
- add user to context

#### Video 23 Video Upload
- bucket config
- aws sdk

#### Video 24 Video Upload 2
- send the video to aws
- axios

#### Video 25 Save Video
- video details and save to database

#### Resources
***Upload Background***
    - https://s3-us-west-1.amazonaws.com/youtube-clone-assets/upload-background.svg
***Sample Bucket Policy***
```
{
    "Version": "2012-10-17",
    "Id": "S3-Console-Auto-Gen-Policy-1501076877929",
    "Statement": [
        {
            "Sid": "S3PolicyStmt-DO-NOT-MODIFY-1501076877929",
            "Effect": "Allow",
            "Principal": {
                "Service": "s3.amazonaws.com"
            },
            "Action": "s3:PutObject",
            "Resource": "arn:aws:s3:::<your bucket name>/*",
            "Condition": {
                "StringEquals": {
                    "aws:SourceAccount": "056188042019",
                    "s3:x-amz-acl": "bucket-owner-full-control"
                },
                "ArnLike": {
                    "aws:SourceArn": "arn:aws:s3:::<your bucket name>"
                }
            }
        }
    ]
}
```
***Sample Bucket CORS Policy***
```
<?xml version="1.0" encoding="UTF-8"?>
<CORSConfiguration xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
<CORSRule>
    <AllowedOrigin><your website url></AllowedOrigin>
    <AllowedMethod>POST</AllowedMethod>
    <AllowedMethod>PUT</AllowedMethod>
    <AllowedMethod>DELETE</AllowedMethod>
    <MaxAgeSeconds>10000</MaxAgeSeconds>
    <AllowedHeader>*</AllowedHeader>
</CORSRule>
<CORSRule>
    <AllowedOrigin>*</AllowedOrigin>
    <AllowedMethod>GET</AllowedMethod>
    <MaxAgeSeconds>3000</MaxAgeSeconds>
    <AllowedHeader>Authorization</AllowedHeader>
</CORSRule>
</CORSConfiguration>
```

#### Important Links
##### [Apollo 2.0](https://www.apollographql.com/)
##### [Express](https://expressjs.com/)
##### [Babel](https://babeljs.io/)
##### [Passport](http://www.passportjs.org/)
##### [Create React App](https://github.com/facebookincubator/create-react-app)
##### [Material UI](https://material-ui-next.com/)
##### [AWS Credentials Docs](http://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/setting-credentials-node.html)
##### [AWS Javascript SDK Docs](http://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/welcome.html)