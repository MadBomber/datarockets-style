# Change Log

The format is described in [Contributing notes](CONTRIBUTING.md#changelog-entry-format).

## master (unreleased)

## 0.9.0 (2020-05-27)

### Changed

* **(Breaking)** Drop support for Ruby 2.3. ([@r.dubrovsky][])

* Update rubocop to '0.84.0'. ([@r.dubrovsky][])
  * Enable new cops `Lint/RaiseException` and `Lint/StructNewOverride`. Cops were added in version `0.81`.
  * Enable new cops `Layout/SpaceAroundMethodCallOperator` and `Style/ExponentialNotation`. Cops were added in version `0.82`.
  * Enable new cops `Layout/EmptyLinesAroundAttributeAccessor` and `Style/SlicingWithRange`. Cops were added in version `0.83`.
  * Enable new cop `Lint/DeprecatedOpenSSLConstant`. Cop was added in version `0.84`.

* Update rubocop-rails to `2.5.2`.
* Update rubocop-rspec to `1.39`.
* Update `activesupport` for fixing security issues.

## 0.8.1 (2020-03-02)

### Changed

* Update rubocop to `0.80.1`.

## 0.8.0 (2020-02-20)

### Added

* Add `Style/NestedInterpolation` cop. ([@r.dubrovsky][])

### Changed

* Update rubocop to `0.80.0`. ([@r.dubrovsky][])
  * Add `Style/HashEachMethods`, `Style/HashTransformKey`, `Style/HashTransformValues` cops.
  * [#7641](https://github.com/rubocop-hq/rubocop/issues/7641): Remove `Style/BracesAroundHashParameters` cop.

* Update rubocop-rspec to `1.38.1`.
  * Add RSpec/RepeatedExampleGroupBody cop. ([@ula][])
  * Add RSpec/RepeatedExampleGroupDescription cop. ([@ula][])

* Enable `rubocop-rails` cops for rails config. ([@ula][])
* Setup `Style/Documentation` for rails config. ([@r.dubrovsky][])
* Setup `Style/ClassAndModuleChildren` cop. ([@r.dubrovsky][])
* Enable `RSpec/LetSetup` cop. ([@r.dubrovsky][])

## 0.7.0 (2020-01-27)

### Added

* [#130](https://github.com/datarockets/datarockets-style/issues/130): Add Layout/ArrayAlignmentExtended cop ([@nikitasakov][])

### Changed

* Update rubocop to `0.79.0`.
* Update rubocop-rspec to `1.37.1`.
* Add notes for setting up Rspec configuration for fixing Rspec internal style issues. ([@r.dubrovsky][])
* [#58](https://github.com/datarockets/datarockets-style/issues/58): Disable `RSpec/LetSetup` cop by default. ([@ula][])

### Fixed

* [#80](https://github.com/datarockets/datarockets-style/issues/80): Allows adding additional files and directories to excluding block for rubocop. ([@nikitasakov][])
* Fix documentation issues. ([@ula][])


## 0.6.2 (2019-12-05)

### Changed

* Update rubocop to `0.77.0`.

## Fixed

* [#137](https://github.com/datarockets/datarockets-style/issues/137): Usage of rubocop 0.77.0 version causes errors. ([@d.kachur][])

## 0.6.1 (2019-11-06)

### Fixed

* [#126](https://github.com/datarockets/datarockets-style/issues/126): Result for ToDo list formatter. ([@r.dubrovsky][])

## 0.6.0 (2019-11-06)

### Added

* [#107](https://github.com/datarockets/datarockets-style/issues/107): Add ToDo list formatter. ([@r.dubrovsky][])

### Changed

* Update rubocop to `0.76`. ([@r.dubrovsky][])
* Change default value for `RSpec/ExampleLength` cop. ([@a.branzeanu][])
* Disable `RSpec/NestedGroups` cop by default. ([@r.dubrovsky][])

## 0.5.0 (2019-10-26)

### Changed

* Split single rubocop config to smaller (for ruby, rails and rspec). ([@r.dubrovsky][])
* Update rubocop to `0.75.1`.
* Update rubocop-rspec to `1.36.0`.
* Use block style for `RSpec/ExpectChange` cop. ([@r.dubrovsky][])
* Add `RSpec/MessageSpies` cop to style guide. ([@r.dubrovsky][])

### Fixed

* Fix `RSpec/DescribedClass`'s error when `described_class` is used as part of a constant. This is part of rubocop-rspec changes.

## 0.4.0 (2019-08-13)

### Changed

* Update rubocop-rspec to `1.35.0`. ([@r.dubrovsky][])
* Use context-dependent style for curly braces around hash params. ([@v.kuzmik][])
* Use leading underscores in cached instance variable name (cop: `Naming/MemoizedInstanceVariableName`). ([@ula][])
* Allow use `for` with `RSpec/ContextWording` cop. ([@r.dubrovsky][])
* Change `Layout/AlignArguments` and `Layout/IndentFirstHashElement` cops for aligning arguments with fixed indentation. ([@r.dubrovsky][])
* Enable `Layout/MultilineMethodCallIndentation` cop for aligning arguments with fixed indentation. ([@r.dubrovsky][], [@ula][])

## 0.3.0 (2019-08-02)

### Changed

* Update rubocop to `0.74.0`. ([@r.dubrovsky][])
* Update rubocop-rspec to `1.34.1`. ([@r.dubrovsky][])
* Move shared rubocop config into `config` directory. ([@r.dubrovsky][])
* Allow writing empty methods in two lines. ([@v.kuzmik][])
* Disable `Style/FrozenStringLiteralComment` cop by default. ([@r.dubrovsky][])

### Fixed

* [#4222](https://github.com/rubocop-hq/rubocop/issues/4222): Disable `Lint/AmbiguousBlockAssociation` for Rspec directory. ([@r.dubrovsky][])
* [#65](https://github.com/datarockets/datarockets-style/issues/65): Exclude `node_modules` from rubocop scope. ([@r.dubrovsky][])

## 0.2.0 (2019-07-17)

### Changed

* Update rubocop to `0.73.0`. ([@r.dubrovsky][])
* Use preferred variable name in rescued exceptions (cop: `Naming/RescuedExceptionsVariableName`). ([@ula][])
* Disable `RSpec/ImplicitSubject` cop for rspec files. ([@r.dubrovsky][])

## 0.1.0 (2019-06-27)

### Added

* Base config with community rules and some basic override rules. ([@r.dubrovsky][], [@aleks][])
* Config is based on rubocop version 0.72.0. ([@r.dubrovsky][])
* Enable `rubocop-spec` cops by default. ([@r.dubrovsky][])
* Enable `Bundler/DuplicatedGem` cop by default. ([@r.dubrovsky][])
* Enable `Bundler/OrderedGems` cop with allowing ordering by groups. ([@r.dubrovsky][])


### Changed

* Change the limit for size of line to 120 symbols. ([@r.dubrovsky][])
* Disable `Metrics/BlockLength` cop for rspec files. ([@r.dubrovsky][])
* Exclude rubocop checking for some config directories. ([@r.dubrovsky][])
* Enable preferring double quotes for string literals. ([@r.dubrovsky][])
* Do not add spaces between hash literal braces (cop `Layout/SpaceInsideHashLiteralBraces`). ([@r.dubrovsky][])
* Prefer normal style for `Layout/IndentationConsistency` cop for Rails apps too. ([@r.dubrovsky][])
* Change style to `variable` for `Layout/EndAlignment` cop. ([@r.dubrovsky][])
* Change style to `with_fixed_indentation` with indentation width 2 for `Layout/AlignParameter` cop. ([@r.dubrovsky][])
* Always ignore hash aligning for key word arguments. (cop: `Layout/AlignHash`) ([@r.dubrovsky][])

[@r.dubrovsky]: https://github.com/roman-dubrovsky
[@aleks]: https://github.com/AleksSenkou
[@ula]: https://github.com/lazycoder9
[@v.kuzmik]: https://github.com/TheBlackArroVV/
[@a.branzeanu]: https://github.com/texpert
[@nikitasakov]: https://github.com/nikitasakov

