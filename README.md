# Bus Tourist Craze — support site

The two pages the app stores require, served by GitHub Pages:

- **Support** — <https://davinoishi.github.io/bus-tourist-craze-support/>
- **Privacy policy** — <https://davinoishi.github.io/bus-tourist-craze-support/privacy.html>

Both URLs are registered in App Store Connect, and the privacy policy URL also
goes in the Google Play Console for the Android version, so **they must not move**. The
privacy policy URL can be edited there at any time, but the support URL is
version-level metadata and changing it after release rides along with a version
update. Renaming this repository would break both.

## This is a copy

The master copy lives in the game's own (private) repository at `store/site/`.
Edit it there and copy the change across, or the two will drift.

This repo is separate because the game repository is private, and GitHub Pages
from a private repo requires a paid plan — and because the game's source should
not become public just to serve two static pages.

## The privacy policy is not boilerplate

It is written against the app's `PrivacyInfo.xcprivacy` manifest, so this page,
the manifest, the "Data Not Collected" nutrition label in App Store Connect and
the Play Console's Data safety form all make the same claims. The app collects
nothing, tracks nothing, and has no server. The only copies of a player's data
outside the device are in the player's own iCloud (iOS 1.1 and later) or the
phone's own Google backup (Android); neither is reachable by us.

If the app ever gains a network call of its own, all of them have to change
together.
