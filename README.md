# CS211_Group_Project

## Course: CS211

## Session: mw 5:35 PM - 6:55 PM

## **Group 15**

## **Contribuators:**
    Isaac Levering  | isaacLevering 
    Presley Henning | PCH0908
    Logan Turner    | ME-Engineer2

## **Repository URL:** https://github.com/isaacLevering/CS211_Group_Project

## **Program Summaries:**
### A. 
    A terminal-based 2048 game written in C++ using standard C++17, functions, loops, conditions, arrays, and text-file input/       output. The goal is to implement both standard 2028 game movements such as:
            1. Slide nonzero tiles as far as possible in the chosen direction.
            2. Merge equal adjacent tiles in the direction of travel. Each tile may participate in only one merge during a move.             A newly merged tile cannot merge again in that move.
            3. Close gaps after merging. Add the value of every newly merged tile to the score.
            4. If the board changed, count one successful move and insert exactly one new 2 in a randomly selected empty cell.               This includes a slide with no merge.
            5. If the board did not change, do not insert a tile or change the score or move count.
            and save, load, new game, scoreboard, help, and exit features.

### B. 
    This program is an implementation of a Luhn Algorithm to check a 16 digit card number for validity. This program will read       the input as a string or character array so leading zeros are preserved, accept exactly 16 characters, each a digit from 0       to 9, reject spaces inside the number, letters, punctuation, and incorrect length with a clear input-format message, and         distinguish malformed input from a correctly formatted number whose checksum fails. This program will meet the following         constraints:
            1. Starting at the rightmost digit, leave that digit unchanged and double every second digit as you move left.
            2. If a doubled value has two digits, add those digits together. Subtracting 9 from a doubled value greater than 9 is
            equivalent.
            3. Sum all the resulting values, including unchanged digits.
            4. The number passes the Luhn checksum exactly when the sum is divisible by 10.

### Task Plan
    Stage   |  Target
    ------- | -----------------------------------------------------------------------------------------------------------
    Week 1  | Set up Git/GitHub and the group repository. Merge setup and left-movement PRs; begin the remaining 2048
            | directions. Share the repository link through Blackboard.
    Week 2  | Merge the remaining 2048 features and save/load after review; complete and review Luhn. Test the integrated
            | code and share a short progress update.
    Week 3  | Complete final tests and documentation. Review and merge the packaging PR, update main, and test the
            | Blackboard ZIP before submission.
           
