## Poker Hands

[![Build Status](https://travis-ci.org/Slemgrim/poker_hands.svg?branch=master)](https://travis-ci.org/Slemgrim/poker_hands)

Simple evaluator for poker hands. Not the fastest, not the shortest but working.
Give a set of 5 cards to poker_hands and get the highest ranking poker hand. 

This package is not for hand comparison and does not resolve identical hands.

## Code Example

```dart
FiveHand fiveHand = new FiveHand([
    new Card(Face.ACE, Suite.SPADE),
    new Card(Face.KING, Suite.SPADE),
    new Card(Face.JACK, Suite.SPADE),
    new Card(Face.TEN, Suite.SPADE),
    new Card(Face.QUEEN, Suite.SPADE)
]);

Hand hand = fiveHand.evaluate();

print(hand); //Hand.ROYAL_FLUSH
```

## Tests

### Run tests 
```
pub run test
```

### Run benchmarks
```
dart benchmark/five_hand_benchmark.dart
```


## Contribution

Feel free to add new evaluators, improve performance of existing ones, or fix bugs. 
Every contribution is welcome.


