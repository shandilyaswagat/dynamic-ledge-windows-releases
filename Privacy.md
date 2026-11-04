# Dynamic Ledge for Windows — privacy

Effective 4 November 2026, starting with Windows version 0.5.2.

Dynamic Ledge does not require an account. Notes, tasks, preferences and pinned references stay in your Windows user folder. Unpinned clipboard history stays in memory. Original files are not uploaded by the tray; choosing Windows sharing sends selected items to the recipient or app you choose.

## App analytics

Dynamic Ledge sends a small set of lifecycle and update events to [TelemetryDeck](https://telemetrydeck.com/): first launch of a new installation, app launches, daily activity, first launch of a newer version, update availability, update attempts and categorized update/check failures. Analytics is enabled without an in-app switch. There is no screen recording or feature-by-feature activity tracking.

Each event contains its event name and time, app version, Windows 10 or 11, x64 or ARM64 architecture, and whether the copy uses Scoop or a portable ZIP. Update events may include the previous or target app version and a broad failure category such as network, invalid release or installation. Raw error messages are never sent.

A random identifier is created in the app's local data folder and hashed with SHA-256 before sending. It is not derived from your name, email, Windows account, hardware identifiers or account credentials. TelemetryDeck further salts and hashes that value. This identifier lets us count participating installations over time; it does not identify a person, and one person using several PCs may count several times. A daily session identifier and a random event identifier support grouping and duplicate analysis.

Event payloads contain no names, email addresses, device names, hardware serial numbers, clipboard contents, notes, file names or paths, calendar details, URLs you visit, account details, coding prompts, approval commands or media titles. The app does not attach an IP address or location to events. As with any internet connection, TelemetryDeck receives network connection information while accepting requests; its handling is described in [TelemetryDeck's privacy policy](https://telemetrydeck.com/privacy/). No claim is made that network transport hides your IP address from the receiving service.

Unsent events are kept locally for up to seven days, with a maximum of 64 events, and removed locally after the server acknowledges them. Sending uses an eight-second timeout and backoff after failures. Reports can include retries or gaps after a crash or prolonged offline use. Update success means a newer version actually launched, rather than only being downloaded. Daily activity means the app was running during an unlocked Windows session; it is not a measurement of continuous interaction.

Deleting the app's local analytics state resets its random identifier; it does not erase already aggregated remote reports and the next launch creates a new identifier. Uninstalling or blocking network access stops further events. Download counts from GitHub are separate from app analytics and include repeat downloads, updates and automated requests.

## Optional connections

Update checks contact the official GitHub release repository. Calendar subscriptions contact the source you configure. Optional lyrics lookup sends track and artist metadata to LRCLIB. Optional coding-tool usage connections query local tools; they are separate from product analytics. Camera preview starts only when requested and stops when closed or the session locks. Windows manages camera permissions. Browser download integration and coding hooks operate only when configured.

For privacy questions, contact the publisher through the official [Talvioh website](https://talvioh.vercel.app/ledge.html). This policy covers the Windows app; other services have their own policies.
