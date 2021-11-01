<img src=".github/Icon-1024.png" width="230" alt="App icon" align="left"/>

<div>
<h2>BetterDummy</h2>
<p>Dummy Display for Macs to Have Custom HiDPI Resolutions<br/>
From one of the maintainers of <a href="https://github.com/MonitorControl/MonitorControl">MonitorControl</a>.<p>
<a href="https://github.com/waydabber/BetterDummy/releases"><img src=".github/macos_badge_noborder.png" width="175" alt="Download for macOS"/></a>
</div>

<hr>

## About

M1 macs tend to have issues with custom resolutions. Notoriously they don't allow sub-4K resolution displays to have HiDPI ("Retina") resolutions even though (for example) a 24" QHD 1440p display would greatly benefit from having an 1920x1080 HiDPI "Retina" mode.

To fix this issue, some resort to buying a 4K HDMI dummy dongle to fool macOS into thinking that a 4K display is connected and then mirror the contents of this dummy display to their actual monitor in order to have HiDPI resolutions available. Others use the built in screens of their MacBooks to mirror to the external display. These approaches have obvious drawbacks and cannot solve all problems.

To fix this problem, BetterDummy creates a virtual dummy display which you can then utilize as a mirror main.

Advantages of BetterDummy over a physical 4K HDMI dummy plug or mirroring your internal display:

- Your HDMI port will remain usable for an other display on the Mac Mini.
- Your internal screen will be available as an extended space on a MacBook (or you can use clamshell mode).
- Does not suffer from issues that prevalent with the physical dummy (like jittery mouse cursor).
- Offers a much wider variety of HiDPI and standard resolutions.
- Works with all aspect ratios, does not depend on what resoluations are recorded in the dummy's EDID/firmware.
- Does not utilize graphics hardware in vain so it is somewhat faster.
- Available instantly.
- It is free ([donations humbly accepted](https://opencollective.com/betterdummy)). :)

Some other possible uses:

- The app is also useful for anybody who is not satisfied with the offered default HiDPI resolutions offered by macOS - as in some cases this could be rather limiting - especially on Wide or UltraWide displays.
- Scale Sidecar resolutions.
- Possible use on a headless Mac for custom resolutions.
- Better quality zooming (`System Preferences`»`Accessibility`»`Zoom`»`Use scroll gesture...`) or High Quality screenshots even on Full HD displays.
- You can use it instead of or alongside other apps that create custom native resolutions.

## Usage

1. Start the app
1. In the app menu choose `Create New Dummy` and select your desired aspect ratio
<br/>
<div align="center">
<img src=".github/menu.png" width="469"/>
</div>
<br/>
  
3. In `System Preferences` -> `Displays` you'll see the new Dummy display (for example `Dummy 16:9`)
4. Activate mirroring. The `Main` display should be the Dummy display
5. Set the Dummy display as `Optimize for`
6. Set `Resolution` as `Scaled` - **you should hold the `Option` key while clicking on the `Scaled` option for a fuller list of resolutions!**
7. You can also click `Show all resolutions` for even more resolutions

<div align="center">
<img src=".github/displayprefs.png" width="550"/>
</div>

9. Select the desired mode.

Notes:

- For most configurations, you'll see HiDPI 'Retina' resolutions in the list by default and see and additional non-HiDPI resolutions marked with a `(low resolution)` tag in the resolution list if `Show all resolutions` is toggled. On some configurations however, you might see HiDPI (high resolution) display modes marked with a `(HiDPI)` tag and standard resolutions _without a tag_.
- You might have to fight a bit with macOS Monterey's new `Displays` tab in Preferences as the `Optimize for` setting tends to reset at random times to the physical display for unknown reasons during changing settings. If this happens, you can set it back to the Dummy.
- You might want to enable the `System Preferences`»`Notifications & Focus`»`Allow Notifications`»`When mirroring or sharing the display` option to allow notifications when mirroring is turned on.

The app saves the dummy display configuratio and automatically restores it upon next restart.

## Installation

- Download the [latest release](https://github.com/waydabber/BetterDummy/releases)
- Move the app to Applications
- Start the app
- Use the app menu bar item to interact.

## Compatibility

The app should be compatible with all M1 class machines (MacBook Air, Mini, 2020 and 2021 MacBook Pros) running Monterey.

_Note about Intel: I did not check on x64 but the app is compiled universal and probably works (happy to update this section based on feedbacks)._

## How can I help?

Some of the options:

- You can contribute to the code (via Pull Requests)
- If you like the app, [you can support the developer](https://opencollective.com/betterdummy/donate). :)
- Don't forget to star the GitHub page!
- Spread the word.

Thank you for your help, it is really appreciated! :)

## Don't forget to check out

**If you like this app, you'll like [MonitorControl](https://monitorcontrol.app) as well!** Control the brightness, volume of your external display like it would be a native Apple display!

## Discord channel

You can join the (mostly self help) discussion on the new [BetterDummy discord channel](https://discord.gg/aKe5yCWXSp).

## Special Thanks

Some of the original code was adapted from [FluffyDisplay](https://github.com/tml1024/FluffyDisplay). Thanks to [@tml1024](https://github.com/tml1024)!
