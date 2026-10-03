# Pattern Pulse

A nine-tile memory game. Watch the flashes and repeat their order. Each successful round adds one beat.

https://raeeskasim1.github.io/pattern-pulse/

## Play

- Choose **Relaxed** or **Quick** before starting.
- Watch the sequence, then repeat it by tapping tiles or pressing **1–9**.
- Clear rounds to increase your best score.
- Use **Restart game** at any time. After a mistake, the expected pattern is revealed.

## Implementation

Plain JavaScript manages idle, showing, input, between-round, and lost states. A run identifier prevents old timers from affecting a restarted game. Input is blocked while the sequence plays.

The best cleared-round score uses localStorage when available. Storage failures do not stop gameplay; the score then lasts only for the current page session. Reduced-motion preferences are respected.

