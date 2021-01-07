## How to delete iOS simulators from the command line with simctl

If you want to free some disk space by removing obsolete simulators after a fresh Xcode update, or to delete a specific device, you can use a `xcrun` subcommand named `simctl delete`:

```
simctl delete <device> [... <device n>] | unavailable | all
```

For example, specifying `unavailable` will delete all simulator devices that are not supported by the current Xcode SDK:

```
xcrun simctl delete unavailable
```