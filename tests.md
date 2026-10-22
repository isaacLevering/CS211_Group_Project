# Unit Tests
//TODO: the required tests for both parts with expected/actual results and pass/fail. Also record the final clean-extraction
build test.

## 2048
Record starting state/input, expected result, actual result, and pass/fail in tests.md. Include board values. Separate the
deterministic movement result from the later random insertion.
  1. Sliding and merging in each of the four directions, including movement through gaps.
  2. Three equal tiles and four equal tiles: no tile merges twice in one move.
  3. A successful slide with no merge: one new 2, one counted move, no score gain.
  4. An unchanged move: no inserted tile and no changed counters.
  5. A full board with a possible merge, and a full board with no possible moves.
  6. Several merges in one move, correct score updates, and reaching the 2048 target.
  7. Save, change the game, and load: exact restoration of all cells and counters.
  8. Missing, incomplete, and malformed saves, including an invalid tile: active state is preserved.
  9. Help, invalid commands, new-game confirmation, and exit behavior.

## Luhn Algorithm
Test input or action               | Expected result
-----------------------------------|------------------------------------------------
4532015112830366                   | Correct format; checksum passes
4532015112830367                   | Correct format; checksum fails
0000000000000018                   | Correct format; leading zeros preserved; passes
453201511283036                    | Reject: 15 digits
45320151128303666                  | Reject: 17 digits
453201511283036X                   | Reject: non-digit
Input containing an internal space | Reject: malformed input
Several checks followed by exit    | Results correct; loop exits cleanly
