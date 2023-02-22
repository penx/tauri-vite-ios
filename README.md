# tauri-vite-ios

An app template, compiled by Tauri + Vite, running on iOS.

Based on [https://github.com/edsky/tauri_yew_ios](tauri_yew_ios).

## Configure

In

- src-tauri/gen/apple/tauri-demo.xcodeproj/project.pbxproj
- tauri-demo/src-tauri/gen/apple/project.yml

Update the following to use your Development Team id.

- DevelopmentTeam = XXX;
- DEVELOPMENT_TEAM = XXX;
- DEVELOPMENT_TEAM: XXX

## Run

Run:

```console
yarn
cd tauri-demo
cargo tauri ios dev
# or
cargo tauri ios build
```

## Known issues

`yarn tauri ios build` will fail with "Bad file descriptor", this can be resolved by using `cargo tauri ios build` instead.
