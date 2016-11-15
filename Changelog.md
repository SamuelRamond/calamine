> Legend:
  - feat: A new feature
  - fix: A bug fix
  - docs: Documentation only changes
  - style: White-space, formatting, missing semi-colons, etc
  - refactor: A code change that neither fixes a bug nor adds a feature
  - perf: A code change that improves performance
  - test: Adding missing tests
  - chore: Changes to the build process or auxiliary tools/libraries/documentation

## master
- fix: [xlsb] simplify setting values and early exit when stepping into an invalid BrtRowHdr
- fix: [xlsb] fix record length calculation

## 0.2.0
- fix: [all] allow range to resize when we try to set a value out of bounds
- docs: less `unwrap`s, no unused imports
- refactor: range bounds is not (`start`, `end`) instead of (`position`, `size`)
- feat: add new methods for `Range`: `width`, `height`, `is_empty`

## 0.1.3
- fix: [xls] better management of continue record for rich_extended_strings

## 0.1.2
- fix: [all] return error when trying to set out of bound values in `Range`
- fix: [xls] do a proper encoding when reading cells (force 2 bytes unicode instead of utf8)
- fix: [xls] support continue records
- fix: [all] allow empty rows iterator

## 0.1.1
- fix: remove some development `println!`

## 0.1.0
- first release!