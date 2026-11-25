<img align="left" width="120" alt="Anvil Point Security" src="https://anvilpointsecurity.com/assets/mark.webp">

Anvil Point Security hardens the software and systems people depend on, and builds the detections that catch an attacker at work. We're a small firm founded in 2026, so in place of client logos we point to work you can check.

<br clear="left"/>

### What we do

- Open-source hardening: small security fixes sent upstream, following each project's own rules, so the fix reaches everyone who runs that code.
- AI-assisted vulnerability discovery: we look for flaws in source code inside isolated sandboxes that we validate first. A finding isn't done until it has a minimal fix and a test that fails before the fix and passes after.
- Detection engineering: rules written in Sigma, with versions for Microsoft Sentinel, Defender XDR, and Elastic. Each one is tested against sample logs, so it fires on the attack and stays quiet on normal activity.
- Threat modeling and infrastructure hardening: what you run, who can reach it, and what to fix first.

### Merged upstream

| Project | What changed | Record |
|---|---|---|
| Mealie | Reported privately: the Paprika import unzipped gzipped recipes with no size limit. The maintainer fixed it in 3.31.0 and published the advisory. | [GHSA-g8p4-w9f8-6cc6](https://github.com/mealie-recipes/mealie/security/advisories/GHSA-g8p4-w9f8-6cc6) |
| Garry's Mod | Traitors can no longer use `ttt_c4_disarm` to disarm a living traitor's C4. | [#2566](https://github.com/Facepunch/garrysmod/pull/2566) |
| Garry's Mod | The `ttt_mute_team` command now ignores modes it doesn't know. | [#2565](https://github.com/Facepunch/garrysmod/pull/2565) |
| Garry's Mod | Spawning a vehicle now checks its `AdminOnly` setting. | [#2564](https://github.com/Facepunch/garrysmod/pull/2564) |
| UnPoller | The web server now masks the InfluxDB token and the OTel API key. | [#1136](https://github.com/unpoller/unpoller/pull/1136) |
| UnPoller | Remote mode now verifies the `api.ui.com` certificate. | [#1135](https://github.com/unpoller/unpoller/pull/1135) |
| Homarr | Failed logins now log the client's IP address. | [#7242](https://github.com/homarr-labs/homarr/pull/7242) |
| Microsoft APM | Package downloads over HTTPS can now trust a corporate CA bundle. | [#2741](https://github.com/microsoft/apm/pull/2741) |
| Gotify | The server now limits the size of a request body. | [#1073](https://github.com/gotify/server/pull/1073) |

In review: Open OnDemand [#6185](https://github.com/OSC/ondemand/pull/6185), which sanitizes the app description on interactive app forms, the same as the form header and help text on that page.

### Disclosure

We follow coordinated disclosure. When we find a vulnerability in code someone else maintains, we report it privately through the channel they ask for and give them 90 days to fix it before we publish. Proofs run only against our own installs, never anyone's live systems. The full policy is at [anvilpointsecurity.com/disclosure](https://anvilpointsecurity.com/disclosure).

Questions about a report we sent go to [security@anvilpointsecurity.com](mailto:security@anvilpointsecurity.com).

[Website](https://anvilpointsecurity.com) | [LinkedIn](https://www.linkedin.com/company/anvil-point-security) | [X](https://x.com/AnvilPointSec)
