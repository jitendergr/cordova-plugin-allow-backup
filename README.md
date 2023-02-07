# cordova-plugin-allow-backup
To allow you to set the allowBackup property of a cordova-android application

```
<platform name="android">
    <edit-config file="AndroidManifest.xml"
                 target="/manifest/application"
                 mode="merge">
        <application android:allowBackup="false"/>
    </edit-config>
</platform>
```

## Installation

By default adding this plugin to your cordova-android project will set the `android:allowBackup` property in the `<application/>` tag to `false`.

```
cordova plugin add cordova-plugin-allow-backup
```

If you want to set the property to `true` use the `ALLOW_BACKUP` environment value.

```
cordova plugin add cordova-plugin-allow-backup --variable ALLOW_BACKUP=true
```
