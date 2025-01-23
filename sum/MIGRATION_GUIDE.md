# Migration Guide

This guide provides instructions on how to migrate your project when upgrading to newer versions of this package.

## Table of Contents
- [Version 1.x to 2.x](#version-1x-to-2x)
- [Version 2.x to 3.x](#version-2x-to-3x)

---

## Version 1.x to 2.x

### Breaking Changes
1. **Changed Function API**
    - `oldFunction()` has been replaced with `newFunction()`.
    - **Fix**: Update your code as follows:
      ```javascript
      // Before
      oldFunction(arg);
 
      // After
      newFunction(arg);
      ```

2. **Renamed Configuration Options**
    - `oldOption` has been renamed to `newOption`.
    - **Fix**: Update your configuration file.

---

## Version 2.x to 3.x

### Breaking Changes
1. **Dropped Support for Node.js v12**
    - Minimum required version is Node.js v14.

2. **Updated Default Behavior**
    - Behavior of `someMethod()` has changed.
    - **Fix**: Use the `legacy` option if you depend on the old behavior:
      ```javascript
      someMethod({ legacy: true });
      ```