# Privacy Policy, Wobble Cake

**Effective date: 2026-09-21**

This policy explains what Wobble Cake collects, and why. Casual Diamond Games makes this game. This
game runs on Android, published under the application ID `com.casualdiamondgames.wobblecake`.

This document describes the game as it stands today. It does not describe every service the
developer might add later.

## What the game collects, and why

The game uses several outside services.

### Advertising: Google AdMob

The game shows interstitial and rewarded video advertisements through the Google Mobile Ads SDK.

Google's Mobile Ads SDK collects data to show and measure advertisements, including an advertising
identifier and other device and app information. See Google's page titled **"Google Play data
disclosure"** for the Mobile Ads SDK,
<https://developers.google.com/admob/unity/privacy/play-data-disclosure>, for the complete list.

The game does not choose what the SDK collects. The game chooses whether the SDK may ask for
advertisements at all, through the consent flow described below.

### Purchases: Unity IAP and Google Play Billing

The game sells two items through Unity IAP, talking to Google Play Billing: "Remove Ads" and a
cosmetic bundle.

A purchase is handled by Google Play. The game itself sees only which of the two items the account
already owns, so it can unlock them. The game does not see payment details, card numbers, or billing
addresses. See Unity's page titled **"Privacy overview, In-App Purchasing"**,
<https://docs.unity.com/en-us/iap/privacy-and-consent/overview>, for what Unity's SDK itself collects
to process a purchase.

### Analytics: Unity Analytics

The game can record gameplay events through the Unity Analytics SDK. Collection is off by default
and only starts if the player agrees, as described in Consent below.

When the player agrees, the game records these events:

| Event | What it records |
|---|---|
| Run started | The random seed the run used. |
| Run ended | Floors cleared, final score, perfect placements, how the run ended, and whether a continue was bought. |
| Run abandoned | Floors cleared and the run's seed, for a run the player quit instead of finishing. |
| Rewarded offer shown | Which rewarded advertisement offer was shown. |
| Rewarded offer finished | Which offer, and whether the player watched it through. |
| Interstitial shown | That an advertisement break was shown, between runs. |

None of these events carry a player's name, email, or any other personal detail; they describe
gameplay only.

See Unity's page titled **"Privacy overview, Analytics"**,
<https://docs.unity.com/en-us/analytics/privacy-and-consent/privacy-overview>, for what the SDK
itself collects about the device and installation to deliver these events.

### Online leaderboard: Unity Gaming Services

The game has a daily challenge with an online leaderboard. The game signs the device in anonymously
(no account, no email, no name) and submits the player's score.

A submitted score carries a small text block called a "run proof": the run's seed and the timing of
the player's taps. This lets a checker confirm the score is real. The proof describes gameplay
inputs only. It does not describe the player.

Once the server-side score check below is enabled for submissions, the run proof text is also sent
to that server for the same check, before the score reaches the leaderboard. This is a new
destination for the same proof data, not a new kind of data.

### Server-side score check: Unity Cloud Code

A Cloud Code module, run by Casual Diamond Games through Unity Cloud Code, checks a submitted
score's proof before it reaches the leaderboard. When active, the run proof text described above
travels to this server, operated by the developer, in addition to the leaderboard itself. The module
receives only the day number, the score, and the encoded proof text; no personal data is involved.

## Consent

The game asks two separate consent questions.

**Advertising consent (EU/EEA/UK and other regions requiring it).** The Google User Messaging
Platform (UMP) shows a consent form the first time the game can request it from Google, before any
advertisement is requested. If consent is required and refused, the game requests no advertisements
for that session. A "Privacy options" row appears in the settings screen whenever Google's SDK
reports that one is required, and the player can reopen the form from there at any time.

**Analytics consent (in-game switch).** The game shows its own consent screen the first time it is
played. The default is refuse until the player agrees. The player can change this answer at any time
from settings. Analytics collection starts only after the player agrees, and stops the moment they
withdraw.

## Children

This game does not target children.

## Data retention and deletion

The game keeps two kinds of data outside the device:

- **An anonymous Unity Gaming Services player ID.** Created on first launch by anonymous sign-in. It
  identifies the installation, not the person.
- **Leaderboard scores**, attached to that anonymous ID.

A settings row ("Delete My Data") deletes a player's data in the app: it revokes the anonymous
player ID on that device. It does not remove the leaderboard score row, which expires at the daily
reset. A player who wants their leaderboard entry removed sooner must contact the developer
directly, at the address below.

## Local data on the device

The game stores a small amount of data on the device itself (coin balance, audio settings, owned
and equipped cosmetics, daily challenge progress, consent answers, chosen language, and onboarding
progress), none of it visible or usable outside the game itself.

**Android backs this data up automatically.** The game leaves Android's auto backup on. This means a
reinstall on the same Google account can restore this saved data, including the consent answers
above, instead of starting fresh. Uninstalling and then clearing the app's storage, rather than only
uninstalling, removes this local data for good.

## Third-party privacy pages

Each SDK above publishes its own data disclosure.

- Google: **"Google Play data disclosure"** for the Mobile Ads SDK,
  <https://developers.google.com/admob/unity/privacy/play-data-disclosure>
- Google: the Google Privacy Policy, which covers Google Play purchases,
  <https://policies.google.com/privacy>
- Unity: **"Privacy overview, Analytics"**,
  <https://docs.unity.com/en-us/analytics/privacy-and-consent/privacy-overview>
- Unity: **"Privacy overview, In-App Purchasing"**,
  <https://docs.unity.com/en-us/iap/privacy-and-consent/overview>
- Unity: **"Game Player and App User Privacy Policy"**, covering Unity Gaming Services
  (Authentication and Leaderboards), <https://unity.com/legal/game-player-and-app-user-privacy-policy>

## Contact

Questions about this policy, or a request to delete data described above, go to:

**cdallport10@gmail.com**

## Changes to this policy

A change to this policy is published on this page with an updated effective date at the top. The
effective date is the record of the current version.
