# Husbandry automata

!!! picture inline end
    ![Header](){ align=right }

The husbandry automata is a turtle with the Husbandry Mechanic Soul upgrade!

This upgrade allows everything that the [Weak automata](https://docs.srendi.de/turtles/weak_automata/) does, and also provides the ability to interact with animals and even capture them.

## Overview

| Peripheral Name           | Interfaces with | Events | Introduced in |
| ------------------------- | --------------- | ------ | ------------- |
| husbandryMechanicSoul     | World           | No     | 0.7r          |

### Peripheral funtions

| Function             | Returns                  | Description                                                    |
| -------------------- | ------------------------ | -------------------------------------------------------------- |
| useOnAnimal()        | true, result or nil, err | Try to use selected item on animal at the front turtle
| inspectAnimal()      | table or nil, err        | Inspect animal at the front of turtle
| searchAnimals()      | table or nil, err        | Returns list of animals around the turtle
| captureAnimal()      | true or nil, err         | Capture animal at the front of turtle
| releaseAnimal()      | true or nil, err         | Release captured animal
| getCapturedAnimal()  | table or nil, err        | Returns information about captured animal

## Changelog/Trivia

0.7r
Added the husbandry automata
