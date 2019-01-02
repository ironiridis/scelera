# sclera

A Golang launcher with these design intents:
* Optionally run as init (pid 1)
* provide persistent configuration storage
* provide http-based configuration and monitoring
* launched processes...
* * are language-independent
* * communicate via stdio
* * get status monitoring, configuration

