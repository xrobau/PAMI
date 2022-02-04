# Introduction

PAMI means PHP Asterisk Manager Interface. As its name suggests its just a
set of php classes that will let you issue commands to an ami and/or receive
events, using an observer-listener pattern.

The idea behind this, is to easily implement operator consoles, monitors, etc.
either via SOA or ajax.

A port for nodejs is available at: http://marcelog.github.com/Nami
A port for erlang is available at: https://github.com/marcelog/erlami

# Abandoned?

As the origin appears to be abandoned, I have forked it and added some things
that I need.

# PHP Versions

Note: PAMI Requires PHP 8.0+

# Installing
Add this library to your [Composer](https://packagist.org/) configuration. In
composer.json:
```json
  "require": {
    "xrobau/pami": "2.*"
  }
```


# LICENSE

Copyright 2016 Marcelo Gornstein <marcelog@gmail.com>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

# Thanks To

* Jason Blank <rumpled at github> for helping in the debugging of the queue
functionality and some other ami inconsistencies.

* Francesco Usseglio Gaudi, for help in debugging the Originate action.

* Matías Barletta, for the vgms support.

* Eli Hunter, for helping in bringing in tls compatibility.

* Freddy dafredmail at googlemail, for his help and testing environment to add
dongle support.

* Joshua Elson for his help in trying and debugging in loaded asterisk servers.

* Jacob Kiers for his help in bringing in and testing async agi functionality,
and CEL event
support.

* Richard Baar for noticing the lack of eof support when reading from socket,
the JabberEvent, and the ScreenName in JabberAction.

* Scot Opell for helping in debugging stream_get_line() in 5.3.9 and 5.3.10

* Brian (wormling) for trying and fixing bugs on asyncagi

* Henning Bragge for helping with newstate event and queues.

* mbonneau for ParkedCall and UnParkedCall events.
