This file is used to record the results of running the various benchmarks in this repo.

If you'd like to add one, please record the test conditions - emulator or platform used, version of BASIC, and whether or not a math pack is being used. Turning off interrupts, using lower-impact display modes or hardware or any other methods of speeding up the system are considered invalid. If you use a new math pack, please run the tests using Atari's math pack as well (if possible) for comparison purposes. Remember to coldboot between runs. Output values from the tests (eg, ahl's "random") are not required - this is about timing, not accuracy. Send in those pull requests!

**classic tests**, seconds rounded to one decimal:

| BASIC              | System               | Math lib | ahl   | broucke | dolkus | sieve |
|--------------------|----------------------|----------|-------|---------|--------|-------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 404   | 14.8    | 14.9   | 314.6 |
| Atari MS BASIC II  | Atari800XMac 6.0     | MS       | 101.9 | 27.3    | 6.3    | n.a   |
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    | 395   | 10.7    | 13.6   | 167.6 |
| BASIC XL 1.03 fast | Atari800XMac 6.0     | Atari    | 395   | 10.5    | 13.5   | 148.1 |
| BASIC XE 4.1       | Atari800XMac 6.0     | Atari    | 388.2 | 10.3    | 13.2   | 227.8 |
| BASIC XE 4.1 ext   | Atari800XMac 6.0     | XE       | 50.4  | 5.8     | 5.2    | 138.9 | (1)
| BASIC XE 4.1 fast  | Atari800XMac 6.0     | XE       | 49.7  | 5.5     | 5.0    | 120.3 |
| Turbo-BASIC XL 1.5 | Atari800XMac 6.0     | Turbo    | 41.6  | 5.9     | 5.1    | 129.8 |

**Rugg/Feldman tests**, seconds rounded to one decimal:

| BASIC              | System               | Math lib | rugg1 | rugg2 | rugg3 | rugg4 | rugg5 | rugg6 | rugg7 | rugg8 |
|--------------------|----------------------|----------|-------|-------|-------|-------|-------|-------|-------|-------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 2.3   | 7.6   | 20.7  | 24.2  | 28.3  | 43.3  | 65.3  | 45.5  |
| Atari MS BASIC II  | Atari800XMac 6.0     | MS       | 1.5   | 9.3   | 17.7  | 20.6  | 21.1  | 35.1  | 55.1  | 8.4   |
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
| Atari MS BASIC II  | Atari800XMac 6.0     | MS       | 94  | 47   | 101   | 96  | 92  | 142   | 102    | 90    | 88      | (2)
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    | 35  | 27   | 28    | 59  | 62  | 33    | 74     | 80    | 42      |
| BASIC XL 1.03 fast | Atari800XMac 6.0     | Atari    | 100 | 140  | 129   | 152 | 105 | 33    | 113    | 118   | 91      |
| BASIC XE 4.1       | Atari800XMac 6.0     | Atari    | 37  | 24   | 27    | 65  | 60  | 33    | 60     | 75    | 40      |
| BASIC XE 4.1 ext   | Atari800XMac 6.0     | XE       | 39  | 29   | 29    | 67  | 80  | 123   | 81     | 105   | 53      |
| BASIC XE 4.1 fast  | Atari800XMac 6.0     | XE       | 130 | 176  | 145   | 206 | 167 | 128   | 129    | 177   | 153     |
| Turbo-BASIC XL 1.5 | Atari800XMac 6.0     | Turbo    | 182 | 154  | 155   | 256 | 154 | 137   | 151    | 169   | 164     |
| Basic++ 1.08       | atari++ 1.83         |          | 138 | 118  | 121   | 183 | 106 | 100   | 155    | 131   | 127     |

**wilkinson looping tests**, seconds rounded to one decimal:

| BASIC              | System               | Math lib | a     | b     | c     | g     | h     |
|--------------------|----------------------|----------|-------|-------|-------|-------|-------|
| Atari Rev C        | Atari800XMac 6.0     | Atari    | 71.6  | 71.6  | 72.1  | 70.1  | 55.9  |
| Atari MS BASIC II  | Atari800XMac 6.0     | MS       | 270.8 | 708.2 | 57.8  | 57.1  | 258.9 | (3, 4)
| BASIC XL 1.03      | Atari800XMac 6.0     | Atari    | 36.9  | 36.9  | 37.5  | 36.9  | 33.5  |
| BASIC XL 1.03 fast | Atari800XMac 6.0     | Atari    | 31.2  | 31.2  | 31.7  | 31.2  | 31.4  | (4)
| BASIC XE 4.1       | Atari800XMac 6.0     | Atari    | 37.1  | 37.1  | 37.2  | 36.7  | 28.7  |
| BASIC XE 4.1 ext   | Atari800XMac 6.0     | XE       | 26.3  | 26.3  | 26.4  | 25.8  | 25.2  |
| BASIC XE 4.1 fast  | Atari800XMac 6.0     | XE       | 21.0  | 21.0  | 21.1  | 20.6  | 22.8  |
| Turbo-BASIC XL 1.5 | Atari800XMac 6.0     | Turbo    | 29.7  | 29.7  | 30.1  | 29.6  | 23.3  |

Notes:

(1) "ext" is with the extensions disk loaded, which replaces the floating point library. The FAST command is enabled by this disk as well, but still has to be separately invoked.

(2) For scruss runs, Atari MS BASIC was tested using the original C64 code, and is therefore not directly compariable to the Atari BASICs. It is, however, suitable for comparison to other MS dialects found on other machines.

(3) These tests run without conversion on MS BASIC. Using `S=TIME` for timing, test a takes 312.4 seconds on a PET, and thus will turn in times within a few seconds of this on the C64 and Apple II. The much better performance of Atari BASIC in these tests is largely due to MS having to re-parse constants and/or perform variable lookups. For illustrating the differences in the underlying concepts in AB and MS, these tests are quite useful.

(4) version b deliberately triggers double precision on MS, while still being within the 10-digit precision of AB.

(4) For BASIC XL and XE, line 1 was added to turn on FAST. Any loss in performance due to longer program length is mooted by the FAST which caches these addresses. As this program is short and only has a single branch, the ~15% improvement in performance is surprising.
