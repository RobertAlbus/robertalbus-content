@@@ PROJECT_TITLE
Markdown-Powered Static Portfolio Website
@@@

@@@ TAGS
Angular, AWS S3, AWS Cloudfront, HTTPS, AWS Route53, Github, Markdown, YAML
@@@

@@@ DESCRIPTION
You're looking at it! Fully JAMified SPA built with Angular & marked-ts
@@@

@@@ DISPLAY
true
@@@

This website is entirely static and does not have a back end. The client application is written in Angular and [all content is stored on Github](https://github.com/RobertAlbus/robertalbus-content). Originally created in 2018, upgraded in 2020 for the external content support. I've extended the markdown parser, [marked-ts](https://github.com/ts-stack/markdown), for this purpose.

Notable features:
* App and content are seperate repos, and both are entirely static
* App is hosted on AWS S3 with Cloudfront, including delivery with TLS
* Content is hosted on github as markdown and yaml
* Implements repository pattern for state management with prudent code re-use by inheriting from a BaseRepository class.
* Uses RXJS Subscriptions and BehaviourSubjects

Shortcomings:
* State is stored in discrete repository items rather than centrally in a state machine
* Application architecture should be further modularized and decoupled
    * This is an upgrade to a legacy project that was one of my first apps. I now live with decisions I made before I knew anything about anything.
s
@@@ REPO
https://github.com/robertalbus
@@@

@@@ LIVE_APP
https://robertalbus.com
@@@
