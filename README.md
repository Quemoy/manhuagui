# `manhuagui`

A cmdline comic downloader for [manhuagui.com](https://tw.manhuagui.com/).
(Forked from chazeon/manhuagui.py)

## Features

- Multiple connections (multi-pages at the same time)
- Auto archive (as .zip) each volume(chapter)
- Auto detect completed volume
- Auto sort volume list
- Progress report
- Auto save download progress of each comic
- Auto download all comics saved locally
- Auto fetch available proxies
- Auto remove dead proxy

## Usage

- If you do not already have Node.js, install it and add to path, such as

````bash
sudo apt-get install nodejs
````

- Before use, first create your own config file

````bash
cp config-default.json config.json
````

- Change any setting you desire by editing `config.json` file.

- Run with

````bash
python3 ./src/main.py -h
````

## Example

- would like to download comics in <https://tw.manhuagui.com/comic/19430/>

````bash
python3 ./src/main.py -i 19430        # fetch all chapter/albums
python3 ./src/main.py -i 19430 -c 20  # start from chapter 21
````

- check and download new comics recorded from local config

````bash
python3 ./src/main.py -a
````

- fetch available proxies and save to config file

````bash
python3 ./src/main.py -u
````

## Known issue
