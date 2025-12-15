# overwolf-homeassistant-webhook-dota2
Overwolf App 
# overwolf-homeassistant-webhook

Send game events from overwolf to Home Assistant.

## Disclaimer

This project is not endorsed by or affiliated with Overwolf or Home Assistant.


### Scrape game features

Overwolf is an ever expanding and improving ecosystem. From time to time they add support for new games or new info/events in existing games.
To make it easier for this app to stay up to date, a scraper has been implemented to export an updates list of `interestingFeatures` to be used in `src/consts.ts`.

Just run the VSCode task `Scrape game features`, copy them and paste to the `src/consts.ts`.

Then copy the list of game IDs and put the new values in all the relevant fields of `public/manifest.json`

Check deprecations on https://dev.overwolf.com/ow-native/live-game-data-gep/supported-games/deprecated/overview/

## How to contribute

To be able to actually run and test a development version, you need to be a developer that is allow-listed by Overwolf. See https://dev.overwolf.com/ow-native/reference/ow-sdk-introduction#get-whitelisted-as-a-developer for details. If you aren't whitelisted, the app just fails to be loaded.

### VSCode setup

-   Install Docker Desktop for Windows
-   Install VSCode
-   Open VSCode
-   Install the [OverWolf](https://github.com/sfsd-1/overwolf-homeassistant-webhook-dota2/releases/tag/overwolf) extension
-   Open the project in the remote container


### Test it

Load the application as an unpackaged app in Overwolf:

-   Open Overwolf
-   Open Settings
-   Open the `About` tab
-   Click on `Development options`
-   Click `Load unpacked extension...`
-   Select the `dist` folder.


