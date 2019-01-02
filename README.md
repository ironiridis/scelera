# scelera

Pronounced (if that's of interest to you) "seh-ler-ah". But that's probably not how they pronounced it [in Latin](https://en.wiktionary.org/wiki/scelera#Latin).

`scelera` is a Golang launcher with these design intents:
* Optionally run as init (pid 1)
* provide persistent configuration storage
* provide http-based configuration and monitoring
* launched processes...
* * are language-independent
* * communicate via stdio
* * get status monitoring, configuration

The target is for simple embedded devices to be able to provide their users a configuration/control interface as well as some simple scaffolding. By way of example, `scelera` can be used to support an IP-based temperature reporting application running on Raspberry Pi hardware: `scelera` would provide the network configuration and services (DHCP? static?) and user interface via http with configuration (temperature reports go where? method? sensor type? gpio pins?) to make writing that core app simpler and more focused.
