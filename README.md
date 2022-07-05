#　Upgrade React-native using react-native CLI

Upgraded from 0.67.4 to 0.69.1
https://react-native-community.github.io/upgrade-helper/?from=0.67.4&to=0.69.1

1. Creating a new application
```zsh
  npx react-native init upgradeProject --template react-native-template-typescript@6.9.6
  cd upgradeProject
```

2. Upgrade
```zsh
  npx react-native upgrade
```

## Files not automatically corrected (or only some of them will be modified)
- package.json  (eslint, metro-react-native-babel-preset, react-test-renderer)

### iOS
- .ruby-version
- Gemfile
- Gemfile.lock
- project.pbxproj

### Android
- MainApplicationTurboModuleManagerDelegate.java (line 44: module name)
- Android.mk (line 13: LOCAL_MODULE)
