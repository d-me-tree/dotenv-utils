# dotenv-utils

A couple of simple bash utility scripts for loading/unloading `.env` files.

## Installation

I store my user scripts in `~/bin`, so that I can run them globally from any directory I am in.  
Below are the steps to set that up:
1. Create `~/bin`
2. Copy `envup` and `envdown` to `~/bin` directory you've created.
3. Add `~/bin` to `PATH` (I have this in `~/.bash_profile`):  
    ```shell
    export PATH=$PATH:$HOME/bin
    ```


## Usage

```shell
. envup         # To load .env file
. envup custom  # To load .env.custom
```

```shell
. envdown  # To unload .env stored in DOTENV_PATH env var (created by envup)
```

## Credits

Inspired by [this gist comment](https://gist.github.com/mihow/9c7f559807069a03e302605691f85572#gistcomment-3225272).
