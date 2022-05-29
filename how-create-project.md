### Ref

1. https://medium.com/how-to-react/convert-your-existing-react-js-app-to-android-or-ios-app-using-the-ionic-capacitor-a127deda75bd
2. https://capacitorjs.com/docs/getting-started

### Init ionic

1. npx create-react-app react-ionic
2. capacitor.config.json

```
{
  "appId": "io.ionic.nameofyourapp",
  "appName": "nameofyourapp",
  "bundledWebRuntime": false,
  "npmClient": "npm",
  "webDir": "build",
  "cordova": {}
}
```

3. ionic.config.json or npx cap init

```
{
  "name": "react-ionic",
  "integrations": {
    "capacitor": {}
  },
  "type": "react"
}
```

4. npm run build
5. npm install -g @ionic/cli
6. npm install @capacitor/core --save
7. npm install @capacitor/cli --save-dev

### Init Android

1. ionic capacitor add android
2. npx cap open android
3. build and run android studio

#### Init Android Setting Variable Ubunut

1. sudo nano $HOME/.bashrc
2. Set the environment variable: `export CAPACITOR_ANDROID_STUDIO_PATH="path of android-studio/bin/studio.sh"`

### Init Ionic

1. ionic capacitor add ios
2. npx cap open ios
3. Xcode build and run
