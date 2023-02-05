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
