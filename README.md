late_tick
==

## Features

- define `tag/function` for registering after `#tick` handlers
- ⚠ called in `schedule tick`
  - So if you do `/schedule` here, you will be 1 tick behind

### Event Handlers

|Resource Location|description|
|:--|:--|
|`tag/function #minecraft:late_tick/<order>`|called every tick after `#minecraft:tick`<br>The smaller `<order>` is, the later it will be called|


## Usage

## Requirement

## Installation

## License
Creative Commons Zero v1.0 Universal
