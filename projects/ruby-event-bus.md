@@@ PROJECT_TITLE
Ruby Event Bus
@@@

@@@ TAGS
Ruby
@@@

@@@ DESCRIPTION
An exploration of the pub-sub relationship using the Mediator pattern
@@@

@@@ DISPLAY
true
@@@

Plain Ruby implementation of a messaging bus. Objects can register as a publisher and/or subscriber, and the message bus brokers the messages.

Notable features:
* Publishers do not need to have knowledge of subscribers.
* subscribers receive messages automatically from the message bus.

Shortcomings:
* Does not guarantee object delivery
* Does not implement topics, tags, or other filtering mechanisms

@@@ REPO
https://github.com/RobertAlbus/event_bus
@@@

@@@ LIVE_APP
https://robertalbus.com
@@@
