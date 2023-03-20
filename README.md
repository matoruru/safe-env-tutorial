# 🔒 safe-env-sample 🔒
This repository explains how to manage environment variables in local development safely with sample folders([folder1](/folder1), [folder2](/folder2)) with an easy step-by-step tutorial.

## Requirements
To try this repository's sample you need these two commands:

- [direnv](https://direnv.net/docs/installation.html)

   This tool allows us to load/unload environment variables depending on folders. Here's the description from the official page:

   > An extension for your shell. It augments existing shells with a new feature that can load and unload environment variables depending on the current directory.

   Install methods:

   ### macOS
   ```
   brew install direnv
   ```

   ### Ubuntu
   ```
   sudo apt install direnv
   ```

   After installation, you need to add hook for your shell by adding a line in its config:

   ### BASH
   ```
   # ~/.bashrc
   eval "$(direnv hook bash)"
   ```

   ### ZSH
   ```
   # ~/.zshrc
   eval "$(direnv hook zsh)"
   ```

   ### FISH
   ```
   # ~/.config/fish/config.fish
   direnv hook fish | source
   ```

- [envchain](https://github.com/sorah/envchain#installation)

   This tool allows us to store and dump from a secure place such as macOS's **Keychain Access**. Here's the description from the officiel page.

   > allows you to secure credential environment variables to your secure vault, and set to environment variables only when you called explicitly.

   Install methods:

   ### macOS
   ```
   brew install envchain
   ```

   ### Ubuntu (from source):
   ```
   make
   sudo make install
   cp ./envchaing ~/bin
   ```

## What each folders describe?
Once you instaled 2 requirements, you can see how it switches environment variables depending on the current folder by moving between `folder1` and `folder2`. Let's proceed to the tutorial below:

## Tutorial 💪

