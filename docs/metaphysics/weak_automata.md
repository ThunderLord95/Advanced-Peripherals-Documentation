# Weak automata

!!! picture inline end
    ![Header](){ align=right }

Weak automata is a turtle with the weak mechanic soul upgrade!

It provides several abilities:

- Digging a block with a tool;
- Clicking on a block with an item or an empty hand;
- Sucking up items around it, all or specific;
- Detecting items around it;
- Detecting blocks and entities in a line;
- Charging the turtle with an RF item inside its inventory;

<br><br><br><br><br><br>

## Overview

| Peripheral Name           | Interfaces with | Events | Introduced in |
| ------------------------- | --------------- | ------ | ------------- |
| weakMechanicSoul          | World           | No     | 0.7r          |

### Peripheral funtions

| Function                                          | Returns                  | Description                                                                                          |
| ------------------------------------------------- | ------------------------ | ---------------------------------------------------------------------------------------------------- |
| getFuelLevel()                                    | int                      | Returns stored fuel                                                                                  |
| getFuelMaxLevel()                                 | int                      | Returns max stored fuel                                                                              |
| getConfiguration()                                | table                    | Returns table with related documentation                                                              |
| lookAtBlock()                                     | table or nil, err        | Returns table with block data at the front of turtle                                                  |
| lookAtEntity()                                    | table or nil, err        | Returns table with entity data at the front of turtle                                                |
| digBlock()                                        | true or nil, err         | Tries to dig the block at the front of the turtle (range modifiers also applied) with tool in selected slot |
| useOnBlock()                                      | true or nil, err         | Tries to click on the block at the front of the turtle (range modifiers also applied) with the item in the selected slot |
| scanItems()                                       | table or nil, err        | Returns data about items in range of turtle                                                          |
| collectSpecificItem(string itemName, [int count]) | true or nil, err         | Collects items around turtle by their name                                                            |
| collectItems([int count])                         | true or nil, err         | Collects items around turtle                                                                          |
| feedSoul()                                        | true, result or nil, err | Tries to feed entity in front of turtle to the weak mechanic soul. Soul should be in selected slot |
| chargeTurtle([int fuel])                          | int or nil, err          | Tries to charge the turtle and returns the amount of recived fuel or an error
| getSuckCooldown() | int | Returns current suck item operation cooldown |
| getDigCooldown() | int | Returns current dig block operation cooldown |
| getUseOnBlockCooldown() | int | Returns current use on block operation cooldown |
| getFuelConsumptionRate() | int | Returns current fuel consumption rate |
| setFuelConsumptionRate(int rate) | true or nil, err | Tries to set fuel consumption rate |

## Changelog/Trivia

0.7r
Added the weak automata
