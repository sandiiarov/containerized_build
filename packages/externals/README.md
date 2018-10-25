# Externals package

The root idea of this package is building shared libraries between SPAs. It is like a `vendor.js` file just one difference - splitting `vendor.js` on a few chucks (react.js, lodash.js, etc).

If a developer wants to share React between SPAs he needs to do to:

- `npm install react -E`
- add react to `peerDependencies` section
- `lerna bootstrap --hoist`
- add react to `packages/main/src/packagemap.json`