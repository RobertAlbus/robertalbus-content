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

The main objective of this project is to evaluate hands of cards from a modified suitless deck. Some of the original requirements did not match with typical real life needs of a game of poker. For example, a requirement was to compare the hands of only two players. I chose to implement a more robust and realistic solution in situations like this.

The first step in the comparison algorithm is to determine the hand rank for each player. The frequency distribution of cards in a given hand is used to determine the hand's signature. The signature is essentially a list of integers that represent type of hand. For example, `[32]` represents a full house, and `[2111]` represents a single pair. This is often sufficient for evaluating a winner. If this is not the case and two hands have an identical signature then card values are evaluated to determine a winner.

Notable features:
* 95% test-coverage
* Compares poker hands for N players
* State is tracked in a central state machine
* All other operations are performed with pure functions
* Utilizes Dependency Injection for sharing the State Machine
* Clear module boundaries between each step (input => preprocess => evaluate => output)

Opportunities for improvement:
* Add support for card suits
* I reduced encapsulation for the sake of unit testing at the behest of the interviewer. I would choose to maintain encapsulation for classes.

@@@ REPO
https://github.com/RobertAlbus/fishtank-poker
@@@
