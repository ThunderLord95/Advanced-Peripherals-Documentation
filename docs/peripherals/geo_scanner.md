# Geo Scanner

!!! picture inline end
    ![Header](){ align=right }

The Geo Scanner provides information about blocks around and in the chunk where scanner located.

The Geo scanner has a delay between scans, so you should be prepared for this when creating programs.

<br><br><br><br><br><br>

## Overview

| Peripheral Name     | Interfaces with | Events | Introduced in |
| ------------------- | --------------- | ------ | ------------- |
| geoScanner          | World           | No     | 0.7r          |


| Function            | Returns              | Description                                       |
| ------------------- | -------------------- | ------------------------------------------------- |
| getFuelLevel()      | int                  | Returns stored fuel                               |
| getFuelMaxLevel()   | int                  | Returns max stored fuel                           |
| cost(int radius)    | int                  | Returns cost in RF for scan                       |
| scan(int radius)    | table or nil, reason | Returns data about blocks in radius               |
| getScanCooldown()   | int                  | Returns cooldown for scanner                      |
| chunkAnalyze()      | table or nil, reason | Returns data about how many ores are in the current chunk |
| getConfiguration()  | table                | Returns configuration for this peripheral         |

## Changelog/Trivia

0.7r
Added nbt storage
