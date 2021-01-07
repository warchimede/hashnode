## How to know which architectures are included in an iOS binary framework

Use the the `lipo` command with the `-info` or `-i` option (example using StuffManager.framework):
```sh
lipo -info StuffManager.framework/StuffManager
```
The output will be something like this:
```
Non-fat file: StuffManager.framework/StuffManager is architecture: arm64
```
or
```
Architectures in the fat file: StuffManager.framework/StuffManager are: x86_64 arm64
```
