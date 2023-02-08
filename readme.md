![shellcheck workflow](https://github.com/rickydodd/marco-polo/actions/workflows/push-actions.yml/badge.svg)

# Marco, Polo!
## Brief
Bash script that lets you mark a directory, using `marco`, and then return to that directory at any time (assuming the user has not overwritten the desired marco) with `polo`.

## Installation
1. Create the local user configuration directory.
   ```bash
   mkdir ~/.config/marco
   ```

2. Create the local user binary directory.
   ```bash
   mkdir ~/bin
   ```

3. Clone the contents of the marco-polo repository to the local user binary directory.
   ```bash
   git clone --depth=1 https://github.com/rickydodd/marco-polo ~/bin/
   ```

4. Remove the `.git` and `readme.md` artefacts.
   ```bash
   rm -rf ~/bin/{.git,.github,readme.md}
   ```

5. Set marco to be sourced with every new bash instance.
   ```bash
   echo -e "source ~/bin/marco\n" >> ~/.bashrc
   ```

You can restart your terminal emulator or run the command `source ~/bin/marco`.

## Usage
- In a directory you want to mark, run the following command.
  ```bash
  marco
  ```
- When you want to return to the marked directory, then run the following command.
  ```bash
  polo
  ```
