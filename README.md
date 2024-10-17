# pw

Simple CLI password manager  
Created by [@z-z](https://github.com/z-z)

## Installation

Clone the repository and add the following lines to your `.bashrc` or `.zshrc`:

```shell
export PW_PATH="<path to cloned directory>"
export PATH="$PW_PATH:$PATH"
source $PW_PATH/pass-completions.sh
```

For Linux, ensure the program `xclip` is installed

## Available Commands

- **help**  
  Show a list of available commands

- **list**  
  Show all keys stored in the file

- **add** `<key>` `<value>`  
  Add a new key/value pair

- **del** `<key>`  
  Remove the entry associated with the key

- **get** `<key>`  
  Copy the value for the specified key to the clipboard

- **ssh** `<key>`  
  Copy the value for the specified key to the clipboard and run `ssh <key>`  
  Ensure proper configuration in `.ssh/config`

## Example entry in `.ssh/config`

```
Host <key>
    HostName example.com
    User username
    Port 22
```
