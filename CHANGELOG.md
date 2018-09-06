# Changelog  
All notable changes to this project will be documented in this file.  

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Python PEP 440 Versioning](https://www.python.org/dev/peps/pep-0440/).  

##[Unreleased]  
- tbd  

##[0.1.0a4.dev20180906]  
### Added  
- Added 4 value-range constraint
  - MinExclusive, MinInclusive
  - MaxExclusive, MaxInclusive
- Added a misc constraint: InComponentConstraint
### Changed  
- Fixed some other edge cases so that more tests pass
- 52 tests now passing
- Bumped version number


## [0.1.0a3.dev20180906]  
### Added  
- Added string-based min-length and max-length constraints  
- Added logic-shape constraints (not, or, and, xone)  
- Fixed the or-datatype.test.ttl file, which would never pass due to the nature of how RDFLib parses boolean literals.  
### Changed  
- Fixed a bug in the string-based pattern-match constraint  
- Changed the variable naming convention to more closely match the SHACL spec  
  - Renamed `fails`, `failures`, `f`, etc to "Reports", because failures in SHACL are a different thing, reports are their correct name.  
- Fixed some minor issues to get more tests passing  
- 40 Tests now passing


## [0.1.0a2.dev20180906] - 2018-09-06  
### Added  
- Added full pattern matching ConstraintComponent, with working flags.  
- Result reporting and report generation is implemented  
- Two types of shapes are now implemented (NodeShapes and PropertyShapes)  
- Implicit class targeting on target-less is implemented  
- Basic path traversal on PropertyShapes is implemented  
- Seven key types of ConstraintComponents are added and working  
### Changed  
- Fixed bug in datatype matcher that would cause some tests to fail.  
- Switched to running all tests in the directory, rather than running individual tests.  
- Fixed textual report output to format Literals better (to see how they are wrong).  
- Bug fixes since previous version  
- 10+ tests are passing.  


## 0.1.0a1.dev20180904 - 2018-09-04  
### Added  

- Initial version, limited functionality  

[Unreleased]: https://github.com/RDFLib/pySHACL/compare/v0.1.0a4.dev20180906...HEAD  
[0.1.0a4.dev20180906]: https://github.com/RDFLib/pySHACL/compare/v0.1.0a3.dev20180906...v0.1.0a4.dev20180906 
[0.1.0a3.dev20180906]: https://github.com/RDFLib/pySHACL/compare/v0.1.0a2.dev20180906...v0.1.0a3.dev20180906 
[0.1.0a2.dev20180906]: https://github.com/RDFLib/pySHACL/compare/v0.1.0a1.dev20180904...v0.1.0a2.dev20180906  
