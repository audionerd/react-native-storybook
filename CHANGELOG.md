# CHANGELOG

## v1.1.3

- Remove socket.io and use plain Websockets [PR #17](https://github.com/kadirahq/react-native-storybook/pull/17). Removes JS debugging requirement.

## v1.1.2

- Partially fix hot module reloading [Issue #8](https://github.com/kadirahq/react-native-storybook/issues/8) with [PR #10](https://github.com/kadirahq/react-native-storybook/pull/10)

## v1.1.1

- Build source files and write README

## v1.1.0

- Replace `PreviewContainer` with `PreviewComponent` where the host and port are configurable

## v1.0.4

- Fix socket.io by using a patched socket.io temporarily [PR #2](https://github.com/kadirahq/react-native-storybook/pull/2)

## v1.0.3

- Fix `window.navigator.userAgent` related issue with socket.io [Issue #1](https://github.com/kadirahq/react-native-storybook/issues/1)

## v1.0.2

- Rename storybook command file from `cli.js` to `storybook.js`

## v1.0.1

- Add missing dependency `commander` to package.json file

## v1.0.0

This is the initial non-poc release of `react-native-storybook`. With this release, users can write stories and check them using an ios-simulator. The address of the storybook `localhost:9001` is hardcoded so for now it does not work on real devices or the android simulator. Also it is not contributor friendly. When used with `npm link`, the node_modules directory should be removed when using the ios simulator.

 - Support ability to write stories using `storiesOf` and `add` without using decorators or addons
 - The storybook can be started with `storybook start -h localhost -p 9001` although the port and host should be as given in this example
 - The story preview device can be started with the `react-native run-ios` command but the apps `index.*.js` must be edited (for now)
