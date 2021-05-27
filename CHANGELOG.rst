#########
Changelog
#########
All notable changes to the pathfinder NApp will be documented in this file.

[UNRELEASED] - Under development
********************************
Added
=====

Changed
=======

Deprecated
==========

Removed
=======

Fixed
=====

Security
========

[2.2.4] - 2021-05-27
********************

Changed
=======
- Changed ``setup.py`` to alert when a test fails on Travis.
- Updated ``requirements/dev.txt`` file.

Fixed
=====
- Fixed a bug in parsing metadata of links (fix #64).


[2.2.3] - 2020-07-24
********************

Added
=====
- Added support for automated tests and CI with Travis.
- Added tags decorator to run tests by type and size.
- Added unit tests, increasing coverage to 90%.

Changed
=======
- Improved documentation about NApp dependencies.
- Changed tests structure to separate unit and integration tests.

Fixed
=====
- Fixed package install when creating symlinks.
- Fixed hops addresses in openapi.yml.
- Updated ``run.in`` to include ``networkx`` dependency


[2.2.2] - 2020-03-11
********************
Added
=====
- Log error message when networkx package isn't installed.
- Updated __init__.py file in tests folder to solve bug when running tests.

Fixed
=====
- Fixed Scrutinizer coverage error.
- Fixed some linter issues.


[2.2.1] - 2019-03-15
********************
Changed
=======
- Continuous integration enabled at scrutinizer.

Fixed
=====
- Improve code organization and fix some linter issues.


[2.2.0] - 2018-12-14
********************
Fixed
=====
- Link status (active/inactive) now considered when creating the graph.


[2.1.1] - 2018-06-15
********************
Fixed
=====
- Fixed pathfinder component to use `k-toolbar-item`.


[2.1.0] - 2018-04-20
********************
Added
=====
- Implements Pathfinder ui.

Fixed
=====
- Fix optional parameters (api/kytos/pathfinder/v2):
  - parameter, undesired_links and desired_links must be optional.

[2.0.0] - 2018-03-09
********************
Added
=====
- Support for filters in the output path list:
  - Desired links, which are required in the paths;
  - Undesired links, which cannot be in any path.

Changed
=======
- Code adapted to work with the new topology NApp output.
