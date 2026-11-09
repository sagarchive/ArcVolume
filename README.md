# ArcVolume: fix low HDMI ARC soundbar volume on Android TV

Soundbar too quiet on HDMI ARC? My soundbar forgets its volume every time the power goes off. After a restart it sits at half, even though the TV shows full. ArcVolume is a small Android TV app that sets it back at every start, and works with soundbars and home theatres that support HDMI-CEC.

**[Website and setup steps](https://sagarchive.github.io/ArcVolume/)** · **[Download the APK](https://github.com/sagarchive/ArcVolume/releases/latest/download/ArcVolume.apk)** · **[Report a problem](https://github.com/sagarchive/ArcVolume/issues)**

## Install

1. Connect your soundbar to the TV's HDMI ARC port.
2. Turn on HDMI-CEC on the TV and the soundbar.
3. Copy `ArcVolume.apk` to a USB drive and install it with your TV's file manager. You may need to allow unknown apps first.
4. Open ArcVolume once from your apps.
5. Restart the TV.

Or with adb:

```
adb connect YOUR_TV_IP:5555
adb install ArcVolume.apk
```

Then open it once on the TV.

## Good to know

- It's on at 100% after install. Open it to choose 10% to 100%, or to turn it off.
- You only need to open it once. After that it runs by itself at every TV start.
- It has no internet permission and doesn't need root.
- Tested on a Xiaomi Mi TV (Android 9) with a boAt Aavante HA0304. Other setups are untested, so please report what happens on yours.
- It runs when the TV fully starts. Waking from sleep may not trigger it.

## Licence

Free to install and use. Please don't sell it, repackage it, or publish it as your own. See [LICENSE](LICENSE).
