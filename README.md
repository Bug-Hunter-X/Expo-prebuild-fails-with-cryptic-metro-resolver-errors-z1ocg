# Expo Prebuild Failure: Metro Resolver Issues

This repository demonstrates a common issue encountered when using `expo prebuild` in Expo CLI projects. The problem stems from errors within the `metro-resolver` module, which handles dependency resolution in React Native.

## Problem

The `expo prebuild` command fails, producing confusing error messages that don't directly point to the root cause.  These errors typically relate to missing modules or incorrect module resolution paths.

## Solution

The solution involves carefully reviewing your project's dependencies, package.json, and project structure. Common causes include:

* **Missing dependencies:** Ensure that all necessary packages are installed and listed in `package.json`.
* **Incorrect paths:** Verify that module import paths in your code are correct and point to the actual location of the modules.
* **Mismatched versions:** Check for version conflicts between different packages in your project.
* **Caching issues:** Try clearing the Expo cache using `expo prebuild --clean`
* **Incorrect configuration:** Review the Expo configuration files and ensure they are correctly set up.

## Setup

1. Clone this repository
2. Install dependencies: `npm install` or `yarn install`
3. Try `expo prebuild` and observe the error (bug.js) then apply solution (bugSolution.js) 