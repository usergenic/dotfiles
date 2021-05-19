# dotfiles

These are all the "dotfiles" I'm sharing across systems.  I am using [GNU Stow][1] to symlink these config files into their appropriate location on target machines.

My new machine setup process:

 - Install GNU Stow.
   - On a Mac, I install homebrew first and use `homebrew install stow`.
   - On a Linux box I install it with `apt-get install stow`.
 - Install Git (if needed).
   - It's usually already installed.
 - Clone this repo:
   ```sh
   git clone https://github.com/usergenic/dotfiles ~/dotfiles
   ```
 - Sync the config files:
   ```sh
   source ~/dotfiles/bash/dot-bash_profile_stow
   dotsync
   ```
 - Verify all the root level config files are symlinks and/or remove the ones that aren't, then `dotsync` again.

[1]: https://www.gnu.org/software/stow/
