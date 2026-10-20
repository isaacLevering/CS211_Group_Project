Part B: Luhn checksum validation
  Objective and input
  Write a separate console program that checks a 16-digit number using the Luhn algorithm. Treat this as checksum
  validation: a passing checksum does not establish that a card exists or is authorized for payment.
  Read the input as a string or character array so leading zeros are preserved. Accept exactly 16 characters, each a digit
  from 0 to 9. Reject spaces inside the number, letters, punctuation, and incorrect length with a clear input-format message.
  Distinguish malformed input from a correctly formatted number whose checksum fails.
  Required algorithm
    1. Starting at the rightmost digit, leave that digit unchanged and double every second digit as you move left.
    2. If a doubled value has two digits, add those digits together. Subtracting 9 from a doubled value greater than 9 is
    equivalent.
    3. Sum all the resulting values, including unchanged digits.
    4. The number passes the Luhn checksum exactly when the sum is divisible by 10.
  For example, the synthetic test input 4532015112830366 passes: the transformed values sum to 50. Changing its last digit
  to 7 produces a sum of 51 and fails.
  Functions and interaction
  Separate input-format validation from the checksum calculation. Include a clearly named checkLuhn function and any
  helpers needed. Implement the calculation yourself rather than calling a checksum library or external service.
  Allow the user to check more than one number without restarting the program. Offer a clear exit choice. Reject malformed
  inputs and allow another attempt; handle end of input cleanly. Do not modify the original input while preparing the
  checksum calculation.
  Required Luhn tests
  Test input or action Expected result
  4532015112830366 Correct format; checksum passes
  4532015112830367 Correct format; checksum fails
  0000000000000018 Correct format; leading zeros preserved; passes
  453201511283036 Reject: 15 digits
  45320151128303666 Reject: 17 digits
  453201511283036X Reject: non-digit
  Input containing an internal space Reject: malformed input
  Several checks followed by exit Results correct; loop exits cleanly
  Record expected and actual outcomes in tests.md.
  Explanation and diagrams
  In report.pdf, dry-run 4532015112830366 using a table with the original digit, whether it is doubled, its transformed value,
  and the running sum. State the traversal order and explain the final modulo check.
  Include a flowchart for the Luhn program and a function workflow diagram showing main, input validation, checkLuhn, and
  helpers. Neat hand-drawn diagrams are acceptable.
