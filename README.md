# Windows Safari

- https://github.com/RemoteDebug/remotedebug-ios-webkit-adapter
- https://www.npmjs.com/package/remotedebug-ios-webkit-adapter

---

1. Install [Scoop](https://scoop.sh): `iwr -useb get.scoop.sh | iex`
2. Install [`ios-webkit-debug-proxy`](https://github.com/google/ios-webkit-debug-proxy#installation)
  - `scoop bucket add extras`
  - `scoop install ios-webkit-debug-proxy`
3. `npm install -g vs-libimobile`
4. `npm install remotedebug-ios-webkit-adapter -g`
5. iOS > Settings > Safari > Advanced > Web Inspector
6. Connect and trust
7. `remotedebug_ios_webkit_adapter --port=9000`
8. chrome://inspect/#devices
9. Configure: add `localhost:9000`
10. Find out it doesn't work
11. Try `ios_webkit_debug_proxy` directly

```
Unable to connect to Tomas Hubelbauer's iPhone
  Please verify that Settings > Safari > Advanced > Web Inspector = ON
```

## To-Do

### Wait for the Windows binary release I guess?

https://github.com/google/ios-webkit-debug-proxy/issues/314
