@@@ PROJECT_TITLE
Poker Hand Comparator
@@@

@@@ TAGS
Typescript
@@@

@@@ DESCRIPTION
Algorithm for evaluating poker hands
@@@

@@@ DISPLAY
true
@@@

This was a coding challenge for a job interview. It evaluates hands of cards from a modified suitless deck. The original requirements included comparing the hands of only two players. That's not how poker works, so I made it compare an arbitrary amount of player hands.

This algorithm converts each players hand to a frequency distribution to evaluate hand ranks. In the event that there is an obvious winner then 



Notable features:
* 95% test-coverage
* State is tracked in a central location
* Makes strong use of pure functions
* Shares modules with Dependency Injection
* Clean code and clear module boundaries between each step (input => preprocess => evaluate => output)

Opportunities for improvement:
* Add support for card suits
* I reduced encapsulation for the sake of unit testing at the behest of the interviewer. I would choose to maintain encapsulation for implementation otherwise.

@@@ REPO
https://github.com/RobertAlbus/fishtank-poker
@@@
