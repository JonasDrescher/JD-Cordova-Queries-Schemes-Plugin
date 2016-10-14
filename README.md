# JD-Cordova-Queries-Schemes-Plugin

Cordova / PhoneGap Plugin to work arround Apple's iOS9 requirement that URL Schemes be declared and submitted to Apple (via Info.plist file).

In short, this plugin just whitelists the Url Scheme of the most popular apps on iOS so they will open when linked to. **This is a work around**. You should probably not use this plugin and instead explicitly call out any apps your app might link to. In the event that you don't know what might be linked to, this plugin should be of some use!

## Install

#### Latest version from GitHub

```
cordova plugin add https://github.com/JonasDrescher/JD-Cordova-Queries-Schemes-Plugin.git
```

## Usage

You can add any schemes necessary by just adding another entry in the list (in `plugin.xml`).

```
<config-file target="*-Info.plist" parent="LSApplicationQueriesSchemes">
    <array>
        ...
        <string>yourfavoriteapp</string>
        ...
    </array>
</config-file>
```

## Contributing

If you feel that I've left out an important app, please modify the `plugin.xml` and send me a pull request along with why you think it should be added.

## Platforms

Applies to iOS (9+) only.

## License

[MIT License](http://mit-license.org)
