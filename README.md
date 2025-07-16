# Ultraterminal

Ultraterminal is a shell-based utility that pulls up all available terminal entries from the game Ultrakill. It provides quick access to weapon data, enemy information and an assortment of thematic texts, from the in-game terminal, straight to your terminal.


## Usage

Ultraterminal is invoked from the command line as follows:

```sh
ultraterminal <subcommand> [arguments]
```

### Subcommands

- `weapons <weapon-name>`: Displays information about a weapon.
  - Example: `ultraterminal weapons Revolver`
- `enemies <enemy-name>`: Displays information about an enemy.
  - Example: `ultraterminal enemies Filth`
- `quote <quote-name>`: Displays the text of a quote.
  - Example: `ultraterminal quote Testament-III`


## Install

```sh
git clone https://github.com/TonyWasNotGone/ultraterminal.git
sudo install -m755 ultraterminal/ultraterminal /usr/local/bin
sudo cp -r ultraterminal/{entries,terminalsearch} /usr/local/bin
sudo chmod +x /usr/local/bin/terminalsearch/*
rm -rf ultraterminal
```

## Uninstall

<Uninstall>
  
  ```sh
  sudo rm -rf /usr/local/bin/ultraterminal && sudo rm -rf /usr/local/bin/entries && sudo rm -rf /usr/local/bin/terminalsearch
  ```
</Uninstall>
