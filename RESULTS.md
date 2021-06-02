This file is used to record the results of running the various benchmarks in this repo.

If you'd like to add one, please record the test conditions - emulator or platform used, version of BASIC, and whether or not a math pack is being used. If you use a new math pack, please run the tests using Atari's math pack as well (if possible) for comparison purposes. Please coldboot between runs. Output values from the tests (eg, ahl's "random") are not required - this is about timing not accuracy. Send in those pull requests!

Classic tests, seconds rounted to one decimal:

| BASIC              | System               | Math lib | ahl   | broucke | dolkus | rugg1 | rugg2 | rugg3 | rugg4 | rugg5 | rugg6 | rugg7 | rugg8 | sieve |
|--------------------|----------------------|----------|-------|---------|--------|-------|-------|-------|-------|-------|-------|-------|-------|-------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 404   | 14.8    | 14.9   | 2.3   | 7.6   | 20.7  | 24.2  | 28.3  | 43.3  | 65.3  | 45.5  | 314.6 |
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    | 395   | 10.7    | 13.6   | 1.6   | 3.6   | 16.0  | 15.9  | 18.1  | 28.4  | 39.1  | 44.5  | 167.6 |
| BASIC XL 1.03 fast | Atari800XMac 6.0     | Atari    | 395   | 10.5    | 13.5   | 1.4   | 2.9   | 15.3  | 15.2  | 15.9  | 23.9  | 34.6  | 44.5  | 148.1 |



scruss tests, value for I:

| BASIC              | System               | Math lib | for | goto | gosub | if | fn | maths | string | array | overall |
|--------------------|----------------------|----------|-----|------|-------|----|----|-------|--------|-------|---------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 31  | 21   | 24    | 49 | 46 | 33    | 53     | 56    | 35      |
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    |

