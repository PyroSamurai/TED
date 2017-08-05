# Dev Tips
---
## How to use revision numbers:
* ##### When using git, a program's _version_ should be only be denoted in _commit tags_. Nowhere else.
* ##### The basic version format is: `major.minor.revision`
#### What they are used for:
* 0.00-.99 - pre-release/beta/alpha
* 1.0.0 - initial stable release
* 1.0.1 - bug fix, minor update 
    * Use 1.0.01 format if you plan to have 10+ updates between features
* 1.1.0 - added feature(s)
    * Use 1.01.0 format if you plan to have 10+ feature updates between major versions
* 2.0.0 - big step up, may not be compatible or optimised for version 1.x
###### You can find more info on software revisioning on the [wiki page](http://wikipedia.org/wiki/Software_versioning) which basically says "everybody does it their own way"

---
## What is not an improvement with respect to user-side features:
1. If it takes more steps to achieve than before: not an improvement.
2. If you can achieve no more than what was possible before: not an improvement.
