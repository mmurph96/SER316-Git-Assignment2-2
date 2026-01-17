## Starting Branch Structure:
```
* ab7cd7b (hotfix) Fix randomInt to properly include max value in range
| * 1f23d1c (feature3) Adds hint helper functions and modifies GuessResult method in GameEngine.java
|                       else statement with logic for giving hints.
|/
| * e367776 (feature2) Implement max attempts logic, goodluck message, game over condition,
|                       and adds maxAttempts constant and game over state
| * 5f95961 (dev) Add goodluck message for players
|/
| * f48cf81 (feature1) Add version comment documenting quit feature.
|  Improve user feedback messages for guesses.
|  Add play-again loop functionality.
|  Add ability to quit game with negative number input.
|/
* 45767c4 (HEAD -> documentation, main) Initial Number guessing game
```
## Learning Summary:
- Squash combines several commits into one single commit.
- Cherry-pick allows you to pluck one commit from a branch and apply it to a main branch without disturbing any others.
- Merge combines one branch's changes into your current working branch.
- Feature3 commit was at first messy and not informative; thus we condensed it into one commit.
- Feature2 commits are linear and clearn now after rebase and Feature1 branch was deleted after being merged into dev.
- You would use cherry-pick to import hotfixes to the fundamental core of a code base to continue developing your feature without worrying about other conflicts.
- You would use merge when you want to check conflicts with the dev branch and compare or ensure your feature works with the current up-to-date branch.
- You would use squash when you got carried away with commit messages or were slacking in your formality due to fatigue; so you use squash to clean the commits up and create a monolithic one to replace them.