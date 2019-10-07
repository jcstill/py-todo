<div align="center">
<h3>PY-TODO</h3>
<img src="https://raw.githubusercontent.com/jcstill/py-todo/master/.meta/screenshot.png">

</div>

## Overview
This is an extended version of [py-todo](https://github.com/aesophor/py-todo)

## Dependencies
* python >=3.5 (sys, re, pickle, pathlib, datetime, [dateutil](https://dateutil.readthedocs.io/en/stable))

## Supported Platforms
* Linux
* OSX - Not tested but should work

## Installation
* Manual Installation (Linux)
```
$ git clone https://github.com/jcstill/py-todo.git
$ cd py-todo && sudo cp todo /usr/bin/todo
```

* Manual Installation (OSX)
```
$ git clone https://github.com/jcstill/py-todo.git
$ cd py-todo && cp todo /usr/local/bin/
```

## Usage
```
Usage: /usr/bin/todo <argument>
-a --add                         -- Add a new item.
-e --edit <index>                -- Edit an item.
-org --orgfile <filename>        -- Add org file TODOs.

-c --complete <index>            -- Mark task as completed (keep in list).
-i --incomplete <index>          -- Mark task as incomplete. (default)

-m --move <index> <new index>    -- Move an item from index to new index.
-r --remove <indices...>         -- Remove items by their indices.
-s --sort                        -- Sort items by their remaining days.

-d --detail <index>              -- Show details section of the task
-l --list                        -- List all items. (called if no args passed)

-h --help                        -- Display help message.
-v --version                     -- Display version info.

Note:
Dates and times should be entered in the ISO 8601 standard (month before day).


Configuration Options (See /home/jacob/.config/py-todo/config):
* color = true / false
* detail_mode = true / false
* week_start_day = Sat/Sun/Mon
* time = true / false

```

## Configuration (Optional)
The default config location is `~/.config/py-todo/config`

```
[PY-TODO]
color = true
detail_mode = true
week_start_day = Sun
time = true
```
## License
Available under the [MIT License](https://github.com/aesophor/py-todo/blob/master/LICENSE)
