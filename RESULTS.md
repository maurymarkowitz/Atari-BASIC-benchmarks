This file is used to record the results of running the various benchmarks in this repo.

If you'd like to add one, please record the test conditions - emulator or platform used, version of BASIC, and whether or not a math pack is being used. If you use a new math pack, please run the tests using Atari's math pack as well (if possible) for comparison purposes. Remember to `NEW` or coldboot between runs. Output values from the tests (eg, ahl's "random") are not required - this is about timing, not accuracy. Send in those pull requests!

**classic tests**, seconds rounded to one decimal:

| BASIC              | System               | Math lib | ahl   | broucke | dolkus | sieve |
|--------------------|----------------------|----------|-------|---------|--------|-------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 404   | 14.8    | 14.9   | 314.6 |
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    | 395   | 10.7    | 13.6   | 167.6 |
| BASIC XL 1.03 fast | Atari800XMac 6.0     | Atari    | 395   | 10.5    | 13.5   | 148.1 |
| BASIC XE 4.1       | Atari800XMac 6.0     | Atari    | 388.2 | 10.3    | 13.2   | 227.8 |
| BASIC XE 4.1 ext   | Atari800XMac 6.0     | XE       | 50.4  | 5.8     | 5.2    | 138.9 |
| BASIC XE 4.1 fast  | Atari800XMac 6.0     | XE       | 49.7  | 5.5     | 5.0    | 120.3 |
| Turbo-BASIC XL 1.5 | Atari800XMac 6.0     | Turbo    | 41.6  | 5.9     | 5.1    | 129.8 |

**Rugg/Feldman tests**, seconds rounded to one decimal:

| BASIC              | System               | Math lib | rugg1 | rugg2 | rugg3 | rugg4 | rugg5 | rugg6 | rugg7 | rugg8 |
|--------------------|----------------------|----------|-------|-------|-------|-------|-------|-------|-------|-------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 2.3   | 7.6   | 20.7  | 24.2  | 28.3  | 43.3  | 65.3  | 45.5  |
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    | 1.6   | 3.6   | 16.0  | 15.9  | 18.1  | 28.4  | 39.1  | 44.5  |
| BASIC XL 1.03 fast | Atari800XMac 6.0     | Atari    | 1.4   | 2.9   | 15.3  | 15.2  | 15.9  | 23.9  | 34.6  | 44.5  |
| BASIC XE 4.1       | Atari800XMac 6.0     | Atari    | 1.5   | 4.4   | 16.5  | 16.5  | 20.2  | 30.0  | 43.3  | 44.5  |
| BASIC XE 4.1 ext   | Atari800XMac 6.0     | XE       | 1.4   | 2.7   | 8.7   | 9.0   | 11.3  | 21.1  | 30.1  | 6.1   |
| BASIC XE 4.1 fast  | Atari800XMac 6.0     | XE       | 1.2   | 2.1   | 8.1   | 8.3   | 9.2   | 16.7  | 25.6  | 6.1   |
| Turbo-BASIC XL 1.5 | Atari800XMac 6.0     | Turbo    | 0.9   | 3.1   | 8.2   | 8.9   | 10.0  | 15.6  | 26.2  | 6.1   |

**scruss tests**, value for I, higher is better:

| BASIC              | System               | Math lib | for | goto | gosub | if  | fn  | maths | string | array | overall |
|--------------------|----------------------|----------|-----|------|-------|-----|-----|-------|--------|-------|---------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 31  | 21   | 24    | 49  | 46  | 33    | 53     | 56    | 35      |
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    | 35  | 27   | 28    | 59  | 62  | 33    | 74     | 80    | 42      |
| BASIC XL 1.03 fast | Atari800XMac 6.0     | Atari    | 100 | 140  | 129   | 152 | 105 | 33    | 113    | 118   | 91      |
| BASIC XE 4.1       | Atari800XMac 6.0     | Atari    | 37  | 24   | 27    | 65  | 60  | 33    | 60     | 75    | 40      |
| BASIC XE 4.1 ext   | Atari800XMac 6.0     | XE       | 39  | 29   | 29    | 67  | 80  | 123   | 81     | 105   | 53      |
| BASIC XE 4.1 fast  | Atari800XMac 6.0     | XE       | 130 | 176  | 145   | 206 | 167 | 128   | 129    | 177   | 153     |
| Turbo-BASIC XL 1.5 | Atari800XMac 6.0     | Turbo    | 182 | 154  | 155   | 256 | 154 | 137   | 151    | 169   | 164     |
| Basic++ 1.08       | atari++ 1.83         |          | 138 | 118  | 121   | 183 | 106 | 100   | 155    | 131   | 127     |
