# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
 - Added support for both `.` and `/`-delimited key paths (#24)
 - Added parameter and return types to everything; enabled strict type checks (#18)
 - Added new exception classes to better identify certain types of errors (#20)
 - `Data` now implements `ArrayAccess` (#17)

### Changed
 - All thrown exceptions are now instances or subclasses of `DataException` (#20)
 - Calling `get()` on a missing key path without providing a default will throw a `MissingPathException` instead of returning `null` (#29)
 - Bumped supported PHP versions to 7.1 - 8.x (#18)

## [2.0.0] - 2017-12-21

### Changed
 - Bumped supported PHP versions to 7.0 - 7.4 (#12)
 - Switched to PSR-4 autoloading

## [1.1.0] - 2017-01-20

### Added
 - Added new `has()` method to check for the existence of the given key (#4, #7)

## [1.0.1] - 2015-08-12

### Added
 - Added new optional `$default` parameter to the `get()` method (#2)

## [1.0.0] - 2012-07-17

**Initial release!**

[Unreleased]: https://github.com/dflydev/dflydev-dot-access-data/compare/v2.0.0...main
[2.0.0]: https://github.com/dflydev/dflydev-dot-access-data/compare/v1.1.0...v2.0.0
[1.1.0]: https://github.com/dflydev/dflydev-dot-access-data/compare/v1.0.1...v1.1.0
[1.0.1]: https://github.com/dflydev/dflydev-dot-access-data/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/dflydev/dflydev-dot-access-data/releases/tag/v1.0.0