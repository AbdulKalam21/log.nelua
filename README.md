# log.nelua
A Minimal, small, and simple logging library written in nelua, inspired by rxi's [log.c](https://github.com/rxi/log.c)

## Getting Started
- Copy paste the ``log.nelua`` file or use this repository as a git submodule

## Example
```lua
require "log"

-- a variable just for example purpose
local offset = 500

log.info("The value of the offset is: ", offset)
log.warn("The nelua you are using is not compatible, your nelua version: ", _VERSION)
log.debug("This is some debug text")
log.error("This is an error")
```

## Documentation