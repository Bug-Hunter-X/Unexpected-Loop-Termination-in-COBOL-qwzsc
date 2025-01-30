# Unexpected Loop Termination in COBOL

This repository demonstrates an uncommon bug in COBOL involving unexpected loop termination.  The `PERFORM VARYING` statement, while seemingly straightforward, can lead to unexpected behavior under specific conditions. This example showcases such a scenario and provides a solution.

## Bug Description
The provided COBOL code utilizes a `PERFORM VARYING` loop to iterate ten times. However, due to an `EXIT PERFORM` statement conditionally executed when the loop counter equals 5, the loop terminates prematurely.

## Bug Solution
The solution addresses the premature loop termination by either removing the conditional `EXIT PERFORM` or modifying the loop logic to achieve the intended behavior.  The revised code ensures the loop completes all ten iterations.