# Split one hard commit into two easy commits

## Preferred: Timed kata with easy setup and affordances

Run `./start` to do the kata.

## Alternative: Manual kata setup that leaves a mess when done

There is a small practice repo named `practice-repo` inside this directory.

1. `cd practice-repo`
2. `ln -s git-objects-and-meta .git`
3. `git checkout .`
4. `git show`
5. Split f7ea324d452df3945e7a598d4a194ff26827e068 into two

## Solutions

### Reset, modify, move

1. `git reset HEAD^`
2. Move the modified paragraph back down
3. Commit just the language change
4. Move the paragraph (no modification) and commit saying 'move only'

### Your solution??? Add it here
