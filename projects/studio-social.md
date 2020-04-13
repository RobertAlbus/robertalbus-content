@@@ PROJECT_TITLE
Event Listing Website
@@@

@@@ TAGS
Angular, AWS Lambda,, AWS Cognito, AWS API Gateway, AWS S3, AWS Cloudfront, HTTPS, AWS Route53
@@@

@@@ DESCRIPTION
Custom minimalist CMS for a recurring music event
@@@

@@@ DISPLAY
true
@@@


This application allows event coordinators to log in and upload posters for the upcoming events. This single-asset approach allows the event coordinators to utilize existing event assets and to administer the website with minimal effort and input. 

Notable features:
* Front end client is written with Angular
    * Fast loading SPA
* Back end is entirely serverless technologies from AWS
    * Node 12 Lambda functions
    * Triggered by API Gateway
    * AuthN/authZ and user pool with AWS Cognito
    * Assets are stored in AWS S3
    * Uses AWS Cloudfront for SSL/TLS 1.1 and for HTML, JS, CSS caching

Shortcomings:
* UI does not display placeholder blocks while content is loading
* Images are retreived directly from the asset bucket
    * Publicly accessible bucket is not a best-practice
    * Misses the opportunity to cache image assets with the CDN
    * Images are not optimized in the backend, so a content author could upload gigantic images and impact performance
    * This is the primary focus in the event that this project is revisited
* Back end repo is manually deployed using CDK CLI and should instead have CI/CD pipeline


@@@ REPO
https://github.com/robertalbus
@@@

@@@ LIVE_APP
https://robertalbus.com
@@@
