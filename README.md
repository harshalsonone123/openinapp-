# Open in app doesn't work with external links
Steps to reproduce
-Set Preview Nightly as default browser and "open in app" set to enabled
-Tap on "play.google.com/music/m/Iwgmydz67i636h7aktocev2b7eq?t=NPR_News_Now" in another application (e.g. Gmail)

Expected behavior
-Link opens in a custom tab in Preview Nightly
-If you tap on "open in Firefox Preview Nightly" and then go to browser menu and tap on "open in app", it will open Google Play Music but it will have lost the deep link location

Actual behavior
-Link should open in Google Play Music right away

Device information
Android device: Pixel 4
Fenix version: Latest nightly
┆Issue is synchronized with this Jira Task


I had tested this on Fenix Nightly 200415 (Build #21060608) with Motorola Moto G6 (Android 8) and Pixel 2 (Android 9) and I could reproduce the issue. The link from the description is opened in custom tab.

Verified as fixed on the latest Fenix Nightly 200511 (Build #21320626) with Motorola Moto G6 (Android 8) and Pixel 2 (Android 9). When tapping the link from the description, one is redirect to Google Play to enable and open Google Play Music.

I had filed the following related issue for the custom tab that remains open even if the link is opened in Google Play: #10562.
