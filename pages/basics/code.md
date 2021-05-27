In computer programming, **standard streams** are preconnected input and output communication channels between a computer program and its environment when it begins execution. The three input/output (I/O) connections are called standard input (**stdin**), standard output (**stdout**) and standard error (**stderr**).

CodinGame's model is to communicate with text, via these streams: your program is given inputs (the data needed to solve the problem) in the stdin and you need to print out the requested answer in the stdout.
Hence, one of our taglines being: _"Read stdin, Flush stdout"_

## Protocol

The default code, given in all CodinGame puzzles, already parses the inputs in stdin, does nothing with them and prints a default output in the stdout.

You can find more details about this default code and what to expect from the inputs and how to format your answer at the bottom of any puzzle statement.

## Debugging

You can use the stderr for debugging purposes. Debug messages will show in the console output (at the bottom left).

You can not use breakpoints.