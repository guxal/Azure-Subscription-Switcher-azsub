# Azure Subscription Switcher (azsub)

The Azure Subscription Switcher (`azsub`) is a command-line utility that allows you to interactively change your active Azure subscription using fuzzy search provided by `fzf`. It also provides a convenient way to list all available subscriptions, indicating the current active subscription with an asterisk (*).

## Prerequisites

- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli) installed and configured
- [fzf](https://github.com/junegunn/fzf) installed

## Installation

1. Save the `azsub` script to a file named `azsub` in a directory that is in your `PATH`.
2. Make the script executable by running `chmod +x azsub`.

## Usage

```text
Interactively change the current Azure subscription.

Usage:
  azsub [-l]

Examples:
  # Interactively change the current Azure subscription
  azsub

  # List all subscriptions (indicating current subscription with a '*')
  azsub -l

Flags:
  -l          List all available subscriptions
  -h, --help  Show this help message
```
# Interactively change the current Azure subscription

To change your current Azure subscription interactively, run the azsub command without any arguments:

```bash
azsub
```

This will open a list of your available Azure subscriptions using fzf. You can navigate through the list and select a subscription by pressing Enter. The selected subscription will then be set as the active subscription.

# List all available subscriptions

To list all available subscriptions, run the `azsub` command with the `-l` flag:

```bash
azsub -l
```

This will display a list of your available Azure subscriptions, with the current active subscription marked with an asterisk (*).


# Autor

- ChatGPT4

# Inspired 

- [kubectl-ctx](https://github.com/weibeld/kubectl-ctx) command kubectl ctx 
