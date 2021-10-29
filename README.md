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
```lua 
log.error(...: varargs): void -- Prints the varags to the standard output
```
```lua
log.warn(...: varargs): void -- Prints the varags to the standard output
```
```lua
log.info(...: varargs): void -- Prints the varags to the standard output
```
```lua
log.debug(...: varargs): void -- Prints the varags to the standard output
```
- Set ``DISABLE_LOG_ERROR = true`` or define it when compiling ``-DDISABLE_LOG_ERROR`` to disable logging of errors.
- Set ``DISABLE_LOG_WARN = true`` or define it when compiling ``-DDISABLE_LOG_WARN`` to disable logging of warn.
- Set ``DISABLE_LOG_INFO = true`` or define it when compiling ``-DDISABLE_LOG_INFO`` to disable logging of info.
- Set ``DISABLE_LOG_DEBUG = true`` or define it when compiling ``-DDISABLE_LOG_DEBUG`` to disable logging of debug.
- Set ``DISABLE_LOG_FILE = true`` or define it when compiling ``-DDISABLE_LOG_FILE`` to disable logging to a text file.
- Set ``DISABLE_LOG_COLOR = true`` or define it when compiling ``-DDISABLE_LOG_COLOR`` to disable Colors when logging.
