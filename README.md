# Atari BASIC benchmarks

This repo contains a number of common BASIC benchmarking programs from the early 1980s converted to Atari format and with timing functions added. In recent versions of Atari800Mac, you can simply cut the text and paste into the emulator and then `RUN` them. Remember to `NEW` between runs.

I have attempted to retain the original line numbering pattern where possible, adding the timing functions on new lines. The timers are stored `ST` and `ET`, which do not appear to have been used in any of the benchmarks, in contrast to `S`, `T` and `E`. 

One of Atari BASIC's major performance problems was its slow line-lookup used in `GOTO` and even `FOR/NEXT`. Adding lines to the code will slow these lookups, so the extra lines in these programs will slow their performance *slightly* compared to the originals. While somewhat annoying, the utility of adding internal timing is too useful to ignore and the effect appears to be unmeasureable.

As the timers are outside the loops that are actually performing the benchmark, adding similar timing lines on other platforms should have exactly the same effect on performance. On systems that lack timer functions, changing these to `REM`s will have the same effect, as it is the number of lines that is important, not what is on them.

Note that on the Atari, the "time" is counted in screen cycles, so on PAL machines the final conversion to seconds would be `/50`, not `/60`.

The benchmarks are:

- ahl - The later version of the Creative Computing benchmark. The original from the [November 1983 issue of Creative Computing](https://archive.org/details/creativecomputing-1983-11/page/n269/mode/2up) magazine was later modified to reduce the number of compound statements.

- broucke - Found in an article on the Newell FASTCHIP from the [October/November 1982 issue of ANTIC](https://archive.org/details/1982-10-anticmagazine/page/n15/mode/2up) magazine. The main goal of this test is to compare floating point accuracy, which will prove useful for those improving Atari's notorious math library.

- dolkus - A variation on a sieve from the same ANTIC article. Unlikely to be very useful, but included for historical reasons.

- ruggfeldman - All seven variations of the original [Rugg/Feldman](https://en.wikipedia.org/wiki/Rugg/Feldman_benchmarks) tests, along with the eighth test from PCW. The last test contains various transcendental functions, which will also be useful for math library updates.

- scruss - [scruss's extensive test suite](https://github.com/scruss/bench64) for MS BASIC converted to Atari format by Faicuai. Values are normalized to the C64=100.

- wilkinson_sieve - Version of the sieve converted to Atari format by Bill Wilkinson himself, found in the [February 1985 issue of Compute!](https://archive.org/details/1985-02-compute-magazine/page/n139/mode/2up) magazine. This version uses a manipulated string for storage, as the Atari's 6-byte number format leaves too little room for an array 8192 long. It is not clear whether the lookup/modifications using the string slicing syntax will compare to the numeric array lookup used on other platforms, some experimentation here would be useful.
