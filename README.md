# Atari BASIC benchmarks

This repo contains a number of common BASIC benchmarking programs from the early 1980s converted to Atari format and with timing functions added. In recent versions of Atari800Mac, you can simply cut the text and paste into the emulator and then `RUN` them. Remember to `NEW` between runs.

I have attempted to retain the original line numbering pattern where possible, adding the timing functions on new lines. The timers are stored `ST` and `ET`, which do not appear to have been used in any of the benchmarks, in contrast to `S`, `T` and `E` which are found in a number of them.

One of Atari BASIC's major performance problems was its slow line-lookup used in `GOTO` and even `FOR/NEXT`. Adding lines to the code will slow these lookups, so the extra lines in these programs will slow their performance *slightly* compared to the originals. While somewhat annoying, the utility of adding internal timing is too useful to ignore.

Note that on the Atari, the "time" is counted in screen cycles, so on PAL machines the final conversion to seconds would be `/50`, not `/60`.

The benchmarks are:

- ahl - The 1984 version of the Creative Computing benchmark. The original from the [November 1983 issue of Creative Computing](https://archive.org/details/creativecomputing-1983-11/page/n269) magazine had lines that were over 40 characters, [this version from May 1984](https://archive.org/details/creativecomputing-1984-03/page/n7) separated out some compound statements into separate lines to reduce line length.

- broucke - Found in an article on the Newell FASTCHIP from the [October/November 1982 issue of ANTIC](https://archive.org/details/1982-10-anticmagazine/page/n15/mode/2up) magazine. The main goal of this test is to compare floating point accuracy, which will prove useful for those improving Atari's notorious math library.

- dolkus - A variation on a sieve from the same ANTIC article. Unlikely to be very useful, but included for historical reasons.

- ruggfeldman - All seven variations of the original [Rugg/Feldman](https://en.wikipedia.org/wiki/Rugg/Feldman_benchmarks) tests, along with the eighth test from PCW. The last test contains various transcendental functions, which will also be useful for math library updates.

- faicuai - Faicuai produced a test based on the pattern of [scruss's extensive test suite](https://github.com/scruss/bench64) for MS BASIC. Values are normalized to the C64=100, so a value of 20 means it is 1/5th as fast as a C64 on that test.

- wilkinson_sieve - Version of the sieve converted to Atari format by Bill Wilkinson himself, found in the [February 1985 issue of Compute!](https://archive.org/details/1985-02-compute-magazine/page/n139/mode/2up) magazine. This version uses a manipulated string for storage, as the Atari's 6-byte number format leaves too little room for an array 8192 long. It is not clear whether the lookup/modifications using the string slicing syntax will compare to the numeric array lookup used on other platforms, some experimentation here would be useful.

- wilkinson_loops - six variations, A through F, of a simple looping system from the [September 1982 issue of Compute!](https://archive.org/details/1982-09-compute-magazine/page/n117/mode/2up). The system demonstrates that on some benchmarks, Atari BASIC does just fine. It is not surprising that the author of Atari BASIC would write one that shows it to be fast... Versions D though F are the same as A through C but use long variable names, which has no effect on Atari timing and thus are not duplicated here. Instead, I have added a new version G, which he mentions on page 120 but does not including in the tests. Version H is my own addition, using a FOR/NEXT loop.
