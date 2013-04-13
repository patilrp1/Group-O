This is "bithacks.h" C header file and it contains various macros for bit
manipulations. It's accompanied with "bithacks-test.c", which tests all the
macros.

------------------------------------------------------------------------------
table
Table of contents:
    [1] Macros in bithacks.h file
    [2] The test program bithacks-test.c


[1]-Macros-in-bithhacks.h-file------------------------------------------------

The "bithacks.h" header provides the following macros:

    * B8(x) - turns x written in binary into decimal,
    * B_EVEN(x) - tests if x is even (bithack #1),
    * B_ODD(x) - tests if x is odd (inverse of (bithack #1)),
    * B_IS_SET(x, n) - tests if n-th bit is set in x (bithack #2),
    * B_SET(x, n) - sets n-th bit in x (bithack #3),
    * B_UNSET(x, n) - unsets n-th bit in x (bithack #4),
    * B_TOGGLE(x, n) - toggles n-th bit in x (bithack #5),
    * B_TURNOFF_1(x) - turns off the right-most 1-bit in x (bithack #6),
    * B_ISOLATE_1(x) - isolates the right-most 1-bit in x (bithack #7),
    * B_PROPAGATE_1(x) - propagates the right-most 1-bit in x (bithack #8),
    * B_ISOLATE_0(x) - isolates the right-most 0-bit in x (bithack #9),
    * B_TURNON_0(x) - turn on the right-most 0-bit in x (bithack #10).
    * B_MASKIDENT_0(x) - form a mask that identifies the trailing 0's(bithacks#11).
    * B_COMPLEMENT2_0(x) - form 2's complement of x(bithacks#12). 


[2]-The-test-program-bithacks-test.c------------------------------------------

The test program "bithacks-test.c" tests all the macros above.

You have to first compile it:

    $ gcc bit-hacks-test.c -o bithacks-test

This will create the "bithacks-test" program. Now run it to verify all the
bithacks in bithacks.h:

    $ ./bithacks-test
    All tests OK.


------------------------------------------------------------------------------

