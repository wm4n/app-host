# A git submodule demo (Host app)

## Usage

1. `git clone` this repo

2. `git submodule update --init --remote --recursive` to get submodule' content

3. `git submodule update --remote` to continue update submodule to latest

## For Travis users

1. Turn on `Allow files from this repository to be used in build on other repository` for submodule projects on Travis to make submodule code available

2. add following to .travis.yml to make sure latest code from the branch is used
   ```yml
   install:
     - git submodule update --remote
   ```
