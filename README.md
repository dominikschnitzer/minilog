minilog
=======

A minimal header only C++ logger system

## Minimal Documentation ##
Currently MINILOG only logs to STDERR, however all is in place to log
to files.

Usage in your C++ project:
    #include "minilog.h"
[...]
    MiniLog::current_level() = logINFO;        // set debug level to INFO
[...]

    MINILOG(logDEBUG) << "DEBUG Log message";  // log at debug level
    MINILOG(logINFO) << "INFO Log message";    // log at info level

Would yield: 
    16:20:33.130 INFO: INFO Log message        // show only info level
                                               // output, since DEBUG >
                                               // INFO

