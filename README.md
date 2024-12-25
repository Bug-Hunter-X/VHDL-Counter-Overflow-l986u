# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: an unsigned counter that doesn't handle overflow.  The `counter.vhdl` file contains the buggy code, while `counter_fixed.vhdl` provides a corrected version.

## The Bug

The original code lacks overflow protection. When the counter reaches its maximum value ("1111"), incrementing it results in unexpected behavior, wrapping around to "0000" which might be misinterpreted as resetting.

## The Solution

The corrected code (`counter_fixed.vhdl`) includes an overflow check using a conditional statement, preventing unexpected behavior and providing the intended functionality.
