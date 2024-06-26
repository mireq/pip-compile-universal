## 0.0.6 (2024-06-25)

### Fix

- Correctly handle out of workign directory dependencies

## 0.0.5 (2024-06-24)

### Fix

- Strip comments from included files

## 0.0.4 (2024-06-23)

### Feat

- Replace dependency names in comments
- Copy dependencies to temporary directory

## 0.0.3 (2023-07-04)

### Feat

- Interpret markers inside temporary requirements files

## 0.0.2 (2023-02-07)

### Fix

- Fixed split regex

## 0.0.1 (2023-02-05)

### Feat

- Added .editorconfig
- Added commitizen settings
- Added setup scripts
- Added .gitignore
- Implemented compilation using temporary files
- Added environment markers generator
- Merge specs by versions
- Added requirements parsing
- Implemented compilation step
- Added pip-tools install
- Automatically create virtualenvs
- Updated arguments passed to pip-compile
- Parse requested version

### Fix

- Reset version
- Missing scm settings
- Modified regex to process not annotated files
- Guess oputput filename from input
- Dont't try kill finished process
- Replaced temporary patsh in requirements
- Only lowercase allowed

### Refactor

- Fixed missing code marker
- Simplified split function
- Wrong name for environment markers
