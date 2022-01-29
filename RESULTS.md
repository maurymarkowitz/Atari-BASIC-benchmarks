This file is used to record the results of running the various benchmarks in this repo.

If you'd like to add one, please record the test conditions - emulator or platform used, version of BASIC, and whether or not a math pack is being used. Turning off interrupts, using lower-impact display modes or hardware or any other methods of speeding up the system are considered invalid. If you use a new math pack, please run the tests using Atari's math pack as well (if possible) for comparison purposes. Output values from the tests (eg, ahl's "random") are not required - this is about timing, not accuracy. Send in those pull requests!

**classic tests**, seconds rounded to one decimal:

| BASIC              | System           | Math lib | ahl   | broucke | dolkus | sieve |
|--------------------|------------------|----------|-------|---------|--------|-------|
| Atari Rev C        | A800XMac 6.0     | Atari    | 404   | 14.8    | 14.9   | 314.6 |
| Atari Rev C        | A800XMac 6.0     | FastChip | 143.5 | 11.3    |  9.4   | 257.9 |
| Atari + FASTPROG   | A800XMac 6.0     | Atari    | 404.3 | 14.6    | 14.9   | 306.8 |
| Atari + FASTPROG   | A800XMac 6.0     | FastChip | 143.9 | 11.4    |  9.4   | 262.2 |
| Atari MS BASIC II  | A800XMac 6.0     | MS       | 101.9 | 27.3    |  6.3   | n.a   |
| BASIC XL 1.03      | A800XMac 6.0     | Atari    | 395   | 10.7    | 13.6   | 167.6 |
| BASIC XL 1.03 fast | A800XMac 6.0     | Atari    | 395   | 10.5    | 13.5   | 148.1 |
| BASIC XE 4.1       | A800XMac 6.0     | Atari    | 388.2 | 10.3    | 13.2   | 227.8 |
| BASIC XE 4.1 ext   | A800XMac 6.0     | XE       |  50.4 |  5.8    |  5.2   | 138.9 |
| BASIC XE 4.1 fast  | A800XMac 6.0     | XE       |  49.7 |  5.5    |  5.0   | 120.3 |
| Turbo-BASIC XL 1.5 | A800XMac 6.0     | Turbo    |  41.6 |  5.9    |  5.1   | 129.8 |

**Rugg/Feldman tests**, seconds rounded to one decimal:

| BASIC              | System           | Math lib | rugg1 | rugg2 | rugg3 | rugg4 | rugg5 | rugg6 | rugg7 | rugg8 |
|--------------------|------------------|----------|-------|-------|-------|-------|-------|-------|-------|-------|
| Atari Rev C        | A800XMac 6.0     | Atari    | 2.3   | 7.6   | 20.7  | 24.2  | 28.3  | 43.3  | 65.3  | 45.5  |
| Atari Rev C        | A800XMac 6.0     | FastChip | 2.2   | 6.5   | 19.0  | 18.3  | 21.3  | 36.3  | 55.5  | 14.5  |
| Atari + FASTPROG   | A800XMac 6.0     | Atari    |       |       |       |       |       |       |       |       |
| Atari + FASTPROG   | A800XMac 6.0     | FastChip | 2.3   | 6.6   | 19.2  | 18.4  | 21.7  | 37.1  | 56.3  | 14.5  |
| Atari MS BASIC II  | A800XMac 6.0     | MS       | 1.5   | 9.3   | 17.7  | 20.6  | 21.1  | 35.1  | 55.1  |  8.4  |
| BASIC XL 1.03      | A800XMac 6.0     | Atari    | 1.6   | 3.6   | 16.0  | 15.9  | 18.1  | 28.4  | 39.1  | 44.5  |
| BASIC XL 1.03 fast | A800XMac 6.0     | Atari    | 1.4   | 2.9   | 15.3  | 15.2  | 15.9  | 23.9  | 34.6  | 44.5  |
| BASIC XE 4.1       | A800XMac 6.0     | Atari    | 1.5   | 4.4   | 16.5  | 16.5  | 20.2  | 30.0  | 43.3  | 44.5  |
| BASIC XE 4.1 ext   | A800XMac 6.0     | XE       | 1.4   | 2.7   |  8.7  |  9.0  | 11.3  | 21.1  | 30.1  |  6.1  |
| BASIC XE 4.1 fast  | A800XMac 6.0     | XE       | 1.2   | 2.1   |  8.1  |  8.3  |  9.2  | 16.7  | 25.6  |  6.1  |
| Turbo-BASIC XL 1.5 | A800XMac 6.0     | Turbo    | 0.9   | 3.1   |  8.2  |  8.9  | 10.0  | 15.6  | 26.2  |  6.1  |

**scruss tests**, value for I, 100=C64 performance on that test, higher is better:

| BASIC              | System           | Math lib | for | goto | gosub | if  | fn  | maths | string | array | overall |
|--------------------|------------------|----------|-----|------|-------|-----|-----|-------|--------|-------|---------|
| Atari Rev C        | A800XMac 6.0     | Atari    | 31  | 21   | 24    | 49  | 46  | 33    | 53     | 56    | 35      |
| Atari Rev C        | A800XMac 6.0     | FastChip | 32  | 24   | 26    | 52  | 54  | 77    | 62     | 62    | 64      |
| Atari + FASTPROG   | A800XMac 6.0     | Atari    | 69  | 50   | 58    | 99  | 60  | 33    | 70     | 68    | 58      |
| Atari + FASTPROG   | A800XMac 6.0     | FastChip |     |      |       |     |     |       |        |       |         |
| Atari MS BASIC II  | A800XMac 6.0     | MS       | 94  | 47   | 101   | 96  | 92  | 142   | 102    | 90    | 88      |
| BASIC XL 1.03      | A800XMac 6.0     | Atari    | 35  | 27   | 28    | 59  | 62  | 33    | 74     | 80    | 42      |
| BASIC XL 1.03 fast | A800XMac 6.0     | Atari    | 100 | 140  | 129   | 152 | 105 | 33    | 113    | 118   | 91      |
| BASIC XE 4.1       | A800XMac 6.0     | Atari    | 37  | 24   | 27    | 65  | 60  | 33    | 60     | 75    | 40      |
| BASIC XE 4.1 ext   | A800XMac 6.0     | XE       | 39  | 29   | 29    | 67  | 80  | 123   | 81     | 105   | 53      |
| BASIC XE 4.1 fast  | A800XMac 6.0     | XE       | 130 | 176  | 145   | 206 | 167 | 128   | 129    | 177   | 153     |
| Turbo-BASIC XL 1.5 | A800XMac 6.0     | Turbo    | 182 | 154  | 155   | 256 | 154 | 137   | 151    | 169   | 164     |
| Basic++ 1.08       | atari++ 1.83     |          | 138 | 118  | 121   | 183 | 106 | 100   | 155    | 131   | 127     |

**wilkinson looping tests**, seconds rounded to one decimal:

| BASIC              | System           | Math lib | a     | b     | c     | g     | h     |
|--------------------|------------------|----------|-------|-------|-------|-------|-------|
| Atari Rev C        | A800XMac 6.0     | Atari    | 71.6  | 71.6  | 72.1  | 70.1  | 55.9  |
| Atari Rev C        | A800XMac 6.0     | FastChip | 62.4  | 62.4  | 62.9  | 61.8  | 50.6  |
| Atari + FASTPROG   | A800XMac 6.0     | Atari    |       |       |       |       |       |
| Atari + FASTPROG   | A800XMac 6.0     | FastChip | 63.8  | 63.8  | 64.3  | 63.2  | 51.9  |
| Atari MS BASIC II  | A800XMac 6.0     | MS       | 270.8 | 708.2 | 57.8  | 57.1  | 258.9 |
| BASIC XL 1.03      | A800XMac 6.0     | Atari    | 36.9  | 36.9  | 37.5  | 36.9  | 33.5  |
| BASIC XL 1.03 fast | A800XMac 6.0     | Atari    | 31.2  | 31.2  | 31.7  | 31.2  | 31.4  |
| BASIC XE 4.1       | A800XMac 6.0     | Atari    | 37.1  | 37.1  | 37.2  | 36.7  | 28.7  |
| BASIC XE 4.1 ext   | A800XMac 6.0     | XE       | 26.3  | 26.3  | 26.4  | 25.8  | 25.2  |
| BASIC XE 4.1 fast  | A800XMac 6.0     | XE       | 21.0  | 21.0  | 21.1  | 20.6  | 22.8  |
| Turbo-BASIC XL 1.5 | A800XMac 6.0     | Turbo    | 29.7  | 29.7  | 30.1  | 29.6  | 23.3  |

Notes:

1) FASTPROG adds the Fast-Stack and Fast-Jump patches from the February 1988 Antic magazine, encoded into line 0 and 1 which have to be added to the programs. These improve the performance of loops and branches and generally are only noticable in longer programs where the line lookup performance is significant.

2) The Newell FastChip is a ROM that replaces the original Atari floating point code with improved versions. This has effects on loop performance as well, but is mostly notable in the math tests.

3) For BASIC XL and XE, line 1 was added to turn on FAST.

4) BASIC XE "ext" is with the extensions disk loaded, which replaces the floating point library. The FAST command is enabled by this disk as well, but still has to be separately invoked as in BASIC XL.

5) For scruss runs, Atari MS BASIC was tested using the original C64 code, and is therefore not directly compariable to the Atari BASICs. It is, however, suitable for comparison to other MS dialects found on other machines.

6) The Wilkinson looping tests run without conversion on MS BASIC, which was the design goal. Using `S=TIME` for timing, test a takes 312.4 seconds on a PET and 296.0 for h. Times will be within a few seconds on the C64 and Apple II. The much better performance of Atari BASIC in these tests is largely due to MS having to re-parse constants and/or perform variable lookups. For illustrating the differences in the underlying concepts in AB and MS, these tests are quite useful.

7) Wilkinson test b deliberately triggers double precision on MS, while still being within the 10-digit precision of AB. This is a bit of a cheat.
