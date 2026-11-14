# Privacy Policy — Dweebles: The Holdout

Privacy policy for the iOS game **Dweebles: The Holdout** (bundle ID `app.dweebles.survival`) by MOUD Labs.

The policy lives in [`index.html`](index.html). Turn on GitHub Pages (Settings → Pages → deploy from `main`, root folder) to get a public URL for App Store Connect.

## What the policy is based on

A scan of the `dweebles-backrooms` repo (commit `abef5c4`, Nov 14, 2026) found:

- **Game Center**: sign-in (display name and player ID) and 2–4 player online co-op through `GKMatch`
- **Nearby co-op**: Bonjour and direct TCP on the local network (`NSLocalNetworkUsageDescription`, no TLS); the lobby is advertised under the player's nearby name
- **Proximity voice chat**: microphone (`NSMicrophoneUsageDescription`), on by default in co-op, open only during a match; voice goes guest → host → players in earshot, over Game Center online or directly nearby; nothing is recorded or stored
- **Local storage only**: settings, best rounds, survivor look, selected maps, and the nearby name in `UserDefaults`
- **None of these**: third-party SDKs, analytics, ads, tracking, in-app purchases, or any server of our own
- **External links**: Sketchfab, itch.io, Poly Haven, ambientCG, and Creative Commons credits

**Update the policy** if you add leaderboards, achievements, IAP, analytics, text chat, voice recording, or any server.

## App Store privacy label

With the current build, **Data Not Collected** is still accurate: voice and gameplay data go only between players' devices in real time, and nothing reaches you. Game Center data is handled by Apple, not by you.
