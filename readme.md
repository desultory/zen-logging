# Zen Logging

### @loggify

This decorator can be added to any class to initialize it with a logger, and add extra logging functionality to that class.

The following additional kwargs are handled in __init__:

* `logger` (Logger) Used as the parent logger, if not set, uses the root logger.
* `_log_init` (bool) Can be passed to loggified classes, to enable or disable additional initialization logging.
* `_log_bump` (int) Changes the log level for added loggers.

Loggified classes will also log use of _\_getattribute__, _\_setattr__,  and _\_getitem__.

Functions returned from _\_getattribute__ will automatically log additioanl information such as passed args and results.

### ColorLognameFormatter

A `logging.Formatter` which colors the loglevel portion.
