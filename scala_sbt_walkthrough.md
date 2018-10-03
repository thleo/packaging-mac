## steps to creating a scala packages
1. install homebrew
2. install sbt
3. create package from skeleton using [giter8](https://github.com/MrPowers/spark-sbt.g8)

***

### 1. Installing Homebrew (if on Mac)

1. go to [homebrew website](https://brew.sh/) and follow install instructions
  - make sure you have admin priviledges

*Note: homebrew as terminal profile is just a color change, not actually homebrew*  

- if already installed and you do not have change permissions (`Operation not permitted` *or* `Permission denied`)
  ```bash
  sudo chmod -N file        # Remove ACLs from file
  sudo chmod ugo+rw file    # Give everyone read-write permission to file
  sudo chflags nouchg file  # Clear the user immutable flag from file
  sudo chflags norestricted file  # Remove the SIP protection from file
  ```
  - change ownership of relevant directories with admin level
    `sudo chown -R [youruser] /[my]/[file]/[directory]`
- remove current directory of Homebrew
  ```bash
  # removing current directory before fresh install
  rm /[current]/[directory]/
  ```
***
## About mac terminal

### `ls`
  Different codes will indicate different permissions
  the first letter will indicate whether a file `-` or directory `d` is returned

  There are 3 sequences of 3 characters each indicating permissions for read `r`, write `w`, and execute `x`:
    - the first sequence will indicate permissions for the owner
    - the second sequence will indicate group permissions
    - the last, global permissions
  - `-le`
  - `-lO`
