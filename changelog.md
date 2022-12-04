# Changelog

## [2.1] - 2022-12-06

* Separate the code into source and declarations.
* Fix bug that occurs on callback assertions.

## [2.0] - 2022-09-29

Update the api to use the Mbed OS 6 callback api rather than `FunctionPointer`.

## [1.5] - 2011-01-13

Made the `isr()` protected and made the class a friend of Ticker. Read the
previous state and store when the sample frequency is set so that initial
`assert_deassert_held()` isn't called at startup.

## [1.4] - 2011-01-13

Added an extra overloaded constructor that allows the DigitalIn PinMode to be
passed when the the class is declared. So mode() isn't really needed but is
left in for completeness.

## [1.3] - 2011-01-13

Updated some doxygen comments.

## [1.2] - 2011-01-13

Added ChangeLog.h file.

## [1.1] - 2011-01-13

Fixed some typos.

## [0.1] - 2011-01-13

Initial Release.
