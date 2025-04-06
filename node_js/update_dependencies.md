# How to Update Dependencies

## Step 1: Check Installed Dependencies
```bash
npm outdated
```
This command will check every installed dependency and compare the current version with the latest version in the npm registry. It is printed out into a table outlining available versions.

It is built into npm so there are no additional packages required to download. `npm outdated` is a good place to start for an overview of the number of dependency updates required.

- Current is the current version installed.
- Wanted is the max version of the package according the semver range.
- Latest is the version of the package tagged as latest in the npm registry.

## Step 2: Install Updates
Install updates for every package:
```bash
npm update
```
Keep in mind that with npm update it will never update to a major breaking-changes version. It updates the dependencies in package.json and package-lock.json. It will use the "wanted" version.
To obtain the "latest" version append `@latest` to individual installs, for example npm install `react@latest`.

## Optional: use npm-check-update

For an advanced and customizable upgrading experience, use `npm-check-updates`. This package can do everything `npm outdated` and `npm upgrade` can do with some added customization options. It does require a package installation, however.
To get started, install the npm-check-updates package globally:
```bash
npm install -g npm-check-updates
```
To upgrade dependencies, run:
```bash
ncu --upgrade

// or 
ncu -u
```

- Red = major
- Cyan = minor
- Green = patch
- 
This updates dependencies in only the package.json file and will select the latest version even if it includes a breaking change. With this method, npm install is not run automatically so be sure to run that afterward to update package-lock.json.
To choose your preferred version type, run `ncu --target [patch, minor, latest, newest, greatest]`.
