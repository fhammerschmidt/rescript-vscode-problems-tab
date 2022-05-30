# rescript-vscode bug

This repo is to demonstrate a bug (or at least somewhat unintuitive behavior) of rescript-vscode, where errors would not appear on the problems tab if there is no single file opened for a certain package (or workspace item).

## Setup

1. Have yarn v1 installed
2. `yarn install`

## Steps to reproduce

1. Open this repository in VSCode
2. Make sure the file `app/src/App.res` is NOT opened in VSCode.
3. `yarn build`
4. No error will appear in the "PROBLEMS" tab.
5. If you open the aforementioned `App.res`, it will appear.
6. If you close it, it will disappear again.
