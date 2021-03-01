# mswjs-react-native-failing
Example repository to show the failing msw.js package with React Native

```sh
yarn
yarn start
yarn ios
```

When loading the app it'll recieve this error:

```
error: Error: Unable to resolve module os from <obscured>/AnotherTest/node_modules/msw/native/lib/index.js: os could not be found within the project.

If you are sure the module exists, try these steps:
 1. Clear watchman watches: watchman watch-del-all
 2. Delete node_modules and run yarn install
 3. Reset Metro's cache: yarn start --reset-cache
 4. Remove the cache: rm -rf /tmp/metro-*
  4 |
  5 | var XMLHttpRequest = require('node-request-interceptor/lib/interceptors/XMLHttpRequest');
> 6 | var os = require('os');
    |                   ^
  7 | var tty = require('tty');
  8 | var events_1 = require('events');
  9 | var nodeRequestInterceptor = require('node-request-interceptor');
  ```
