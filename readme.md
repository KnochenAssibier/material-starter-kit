# Material Starter Kit
## A file template to help you get started with Material Components for the Web

This file template sets up the `webpack` configuration and installs the `npm` packages required to get Material Components for the Web up and running. It simply displays a Material button that says "Hello World"!

- View it on [GitHub Pages](https://bonniezhou.github.io/material-starter-kit/)
- View it on [Glitch](https://glitch.com/~material-starter-kit)

## Build this project

### Run locally for development
1. From the root directory, run: 
```
npm install
npm start
```
> Note: This will use `webpack-dev-server` to run the project locally.
2. Point your browser to http://localhost:8080/

### Build for production
1. From the root directory, run: 
```
npm install
npm run-script build
```
> Note: This will update `bundle.js` and `bundle.css` in the `dist/` folder.
2. Open `index.html` in your browser


## Interested in learning more?
Check out the [Material Components for the Web](https://github.com/material-components/material-components-web) documentation to add more components and styling.

Read the full [Getting Started guide](https://github.com/material-components/material-components-web/blob/master/docs/getting-started.md)

[Material Theming](https://material.io/design/material-theming)

*Built with [Material Starter Kit](https://glitch.com/~material-starter-kit) a file template to get you up and running with Material Components for the Web. Remix it and start theming.*

$ git commit
Your browser will now be opened to:
https://oauth2.sigstore.dev/auth/auth?access_type=online&client_id=sigstore&...
[main 040b9af] Signed commit

$ git verify-commit HEAD
tlog index: 2801760
gitsign: Signature made using certificate ID 0xf805288664f2e851dcb34e6a03b1a5232eb574ae | CN=sigstore-intermediate,O=sigstore.dev
gitsign: Good signature from [billy@chainguard.dev]
Validated Git signature: true
Validated Rekor entry: true

brew tap sigstore/tap
brew install gitsign

github.com/sigstore/gitsign@latest

$ gitsign --version
gitsign version v0.7.1

cd /path/to/my/repository
git config --local commit.gpgsign true  # Sign all commits
git config --local tag.gpgsign true  # Sign all tags
git config --local gpg.x509.program gitsign  # Use Gitsign for signing
git config --local gpg.format x509  # Gitsign expects x509 args

git config --global commit.gpgsign true  # Sign all commits
git config --global tag.gpgsign true  # Sign all tags
git config --global gpg.x509.program gitsign  # Use Gitsign for signing
git config --global gpg.format x509  # Gitsign expects x509 args

$ git config --local gitsign.connectorID https://accounts.google.com
$ cat .git/config
[gitsign]
        connectorID = https://accounts.google.com

$ git commit --message="Signed commit"
Your browser will now be opened to:
https://oauth2.sigstore.dev/auth/auth?access_type=online&client_id=sigstore&...
[main 040b9af] Signed commit

$ git verify-commit HEAD
tlog index: 2801760
gitsign: Signature made using certificate ID 0xf805288664f2e851dcb34e6a03b1a5232eb574ae | CN=sigstore-intermediate,O=sigstore.dev
gitsign: Good signature from [billy@chainguard.dev]
Validated Git signature: true
Validated Rekor entry: true

$ git tag v0.0.1
Your browser will now be opened to:
https://oauth2.sigstore.dev/auth/auth?access_type=online&client_id=sigstore&...

error: gpg failed to sign the data
fatal: failed to write commit object

