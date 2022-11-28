@@@ PROJECT_TITLE
Event Listing Website
@@@

@@@ TAGS
Angular, AWS Lambda, AWS Cognito, AWS API Gateway, AWS S3, AWS Cloudfront, HTTPS, AWS Route53
@@@

@@@ DESCRIPTION
Custom minimalist serverless CMS for a recurring music event
@@@

@@@ DISPLAY
true
@@@


This application allows event coordinators to log in and upload posters for the upcoming events. The client application is written in Angular. The back end leverages AWS serverless technologies and Infrastructure as Code.

Notable features:
* Front end client is written with Angular
    * Fast loading SPA
* Back end is entirely serverless technologies from AWS
    * Node 12 Lambda functions
    * Triggered by API Gateway
    * AuthN/authZ and user pool with AWS Cognito
    * Assets are stored in AWS S3
    * Uses AWS Cloudfront for SSL/TLS 1.1 and for HTML, JS, CSS caching

Opportunities for improvement:
* Set up CI/CD for both front end and back end repos
* Add asset optimization for images
* Access the asset through a media delivery subdomain instead of from the bucket directly.
    * Enable asset caching in addition to the current document caching with the existing CDN
    * This approach would adhere to best practices


@@@ LIVE_APP
https://habitatstudiosocial.com
@@@
