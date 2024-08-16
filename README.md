# Countdown #

[Demo](https://MERNCraft.github.io/countdown)

This CSS-only mini-game demonstrates using CSS counters in two different ways: 

1. To provide a countdown, in association with a @keyframes animation
2. To ensure that words are spelt in the correct singular or plural form

In effect, the countdown starts at "10 seconds" (with a final "s") and reaches "1 second" (with no final "s"). This is thanks to a @counter-style with symbols for `1` and `2`. The symbol for `2` is "\00A0seconds", where "\00A0" is rendered by CSS as a non-breaking space. The symbol for `1` lacks the final "s".

The `timer` animation is launched with an `animation-play-state` of `paused`, and this is set to `running` if the radio button is checked. This decrements a `counter` named `countdown` from `10` down to `0`. If the animation is not paused before it ends, it shows a `<div>` with a red background and an ominous message.