dotfiles-local
==============

My local dotfiles based on
[thoughtbot/laptop](https://github.com/thoughtbot/laptop),
[thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and managed with
[thoughtbot/rcm](https://github.com/thoughtbot/rcm).

Installation
------------

### Laptop

  ```
  curl --remote-name https://raw.githubusercontent.com/thoughtbot/laptop/master/mac
  sh mac 2>&1 | tee ~/laptop.log
  ```

### Dotfiles

  ```
  git clone https://github.com/thoughtbot/dotfiles.git ~/dotfiles
  git clone https://github.com/nhutdm/dotfiles-local.git ~/dotfiles-local
  env RCRC=$HOME/dotfiles/rcrc rcup
  ```

Update
------

After making your personal customizations to dotfiles-local, you can safely
re-run these commands multiple times to update.

  ```
  rcup
  sh mac 2>&1 | tee ~/laptop.log
  ```
