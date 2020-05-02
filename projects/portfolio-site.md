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

This is an upgrade to a legacy project that was one of my first apps. I now live with decisions I made before I knew anything about anything.

Notable features:
* App and content are seperate repos, and both are entirely static
* App is hosted on AWS S3 with Cloudfront, including delivery over HTTPS
* Content is hosted on github as markdown and yaml
* Implements repository pattern for state management with code re-use by inheriting from a BaseRepository class.
* Uses RXJS Subscriptions and BehaviourSubjects

Opportunities for improvement:
* Derive top menu programmatically from the content metadata
* Make the site header and title configurable
* Decouple the application from "types" of content, as it is all essentially the same
* Create a lightweight content management client in the same directory as the content files, with a build command to generate the metadata spec, content settings, and folder structure.

@@@ REPO
https://github.com/robertalbus
@@@

@@@ LIVE_APP
https://robertalbus.com
@@@
