# Devcontainer for Zephyr

## Prerequisites

- docker can be used with user privileges. Test with `docker ps` and see if you observe an error.
- VS Code with devcontainer extension

## Usage

This repo will live next to your `zephyr` repository in your workspace. Therefore you need to create your workspace folder first and then clone this repository into it.

1. Create a folder to be your zephyr workspace `mkdir workspace`
2. Switch to that folder `cd workspace`
3. Clone this repository `git clone ...`
4. Open the just cloned folder with VS Code
5. If not prompted select `Reopen in Container` from the command palette
6. Wait for the container to be pulled and created
7. Open a terminal in VS Code. Be sure to be in `/workspace`
8. Start Zephyr developing by using `west` to initialize the workspace with `west init -m https://github.com/zephyrproject-rtos/zephyr --mr v3.7.0` and then `west update` to fetch all the other repositories
