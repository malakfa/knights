# Knights and Knaves Puzzle Solver

## Overview

This project aims to solve Knights and Knaves puzzles, which are logical puzzles introduced by logician Raymond Smullyan. In these puzzles, characters known as knights always tell the truth, while knaves always lie. The objective is to determine the identities of characters based on the statements they make.

## Puzzle Representation

To represent these puzzles using propositional logic, we define the following symbols:

- Let \( K_i \) represent "Character \( i \) is a knight."
- Let \( S_i \) represent "Character \( i \) says a certain statement is true."

Using these symbols, we can express the truth value of each statement as follows:

- If \( K_i \) is true, then \( S_i \) must also be true, as knights always tell the truth.
- If \( K_i \) is false, then \( S_i \) must be false, as knaves always lie.

## Example

Consider a simple puzzle with one character, A, who says "I am both a knight and a knave." We represent this statement as \( S_A \), and the truth value of \( S_A \) will depend on the truth value of \( K_A \).

If \( K_A \) is true (A is a knight), then \( S_A \) must also be true. But since the statement cannot be true (A cannot be both a knight and a knave), we conclude that \( K_A \) must be false (A is a knave).

## Dependencies

This project relies on a model-checking algorithm to solve the puzzles. Any model-checking algorithm capable of handling propositional logic can be used. We can use existing libraries or implement our own model-checking algorithm.

## Usage

To solve a Knights and Knaves puzzle:
1. Represent the puzzle statements using propositional logic symbols \( K_i \) and \( S_i \).
2. Implement a model-checking algorithm to determine the truth values of \( K_i \) based on the statements \( S_i \).

## Future Enhancements

- Implement a user-friendly interface to input puzzles and view solutions.
- Enhance the solver to handle more complex puzzles with multiple characters and statements.
- Optimize the solver for better performance on larger puzzles.

