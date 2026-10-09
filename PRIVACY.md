# FrameFit Privacy Policy

Last updated: October 9, 2026

This policy describes FrameFit 2.18.3, maintained by Band
([band-band on GitHub](https://github.com/band-band)).

## What FrameFit does

FrameFit lets users view supported web video players in a compact browser window,
the current tab, native Picture-in-Picture, or linked Multi-view windows. It processes the information below
on the user's device to provide these features.

## Information processed locally

- **Website addresses:** FrameFit reads the current page address and domain to apply
  per-site settings, validate extension requests, and handle navigation. Domains
  that the user disables are saved as preferences. FrameFit does not maintain a log
  of visited pages or store a history of video URLs.
- **Website content:** FrameFit identifies video elements, player containers, controls,
  and embedded frames. It reads element geometry and playback state to select and
  resize the player. It does not capture, download, record, or upload video or audio.
- **User interaction:** FrameFit handles fullscreen clicks, supported keyboard
  shortcuts, pointer position, page focus, and scroll position to select a player
  and restore the page. It does not keep an interaction log or record text entered
  into forms, chat, or password fields.
- **Preferences:** Enabled status, viewing mode, disabled website domains, and menu
  theme, the Alt-click menu switch, and remembered fullscreen choices per website
  are saved using Chrome's local extension storage. FrameFit does not use
  Chrome's storage.sync service.
- **Window restoration:** Window identifiers, tab position, pinned state, window
  bounds, and maximized state are kept in Chrome's session storage so the tab can
  return to its original window. Restoration records are removed when restoration
  completes or the associated tab is closed. Session storage is temporary.
- **Linked videos:** Video-page titles (up to 1024 characters), website domains,
  group membership, preview slots, layout, horizontal/vertical spacing, and window geometry (including Custom positions and sizes) are kept
  in session storage to display the menu and move linked windows. Layout changes
  use the current screen's available dimensions. Optional audio focus also keeps
  previous tab mute settings in session storage so they can be restored. Group
  membership entries are removed on detach, return to tab, manual tab move, or
  window close. Detaching or unlinking leaves the basic title, domain, and window
  restoration records in session storage while that player remains in Tab View,
  so it can appear in Available windows and return to its original tab. Those
  records are removed on return to tab, manual tab move, window close, or session
  end. Group records are removed when unlinked or no members remain.
  If Chrome temporarily rejects restoring audio, the affected recovery records
  remain until a later retry succeeds or the associated tab is closed. Return to
  tab still completes without waiting for that audio retry.
- **Multi-view:** Original player tabs run in native windows, with a separate
  control window. Its tab/window identifiers and source anchor are held in
  Chrome session storage. Group membership, movement preference, geometry,
  titles, domains, and prior audio settings use the linked-video records above.
  Closing the controls leaves original players running. Current Multi-view does
  not capture or copy video. Upgrading releases any retired capture session and
  restores its previous audio and owned source-window state.

## Transmission and sharing

FrameFit has no developer-operated backend, analytics, advertising, or telemetry.
The extension does not send the information above to the developer or external
servers, sell it, or use it for advertising, profiling, creditworthiness, or lending.
It does not request an account, payment details, health information, precise location,
or authentication credentials. Its executable code is included in the extension package.

Videos and websites you visit still communicate with their own providers under their
own privacy policies. Chrome's services, the Chrome Web Store, and GitHub are also
governed by their respective privacy policies. Information you voluntarily submit in
a GitHub issue is separate from extension operation and may be publicly visible.

## Retention and control

Preferences remain in local extension storage until changed, cleared, or removed
with the extension. Disabling a website adds its domain to the local disabled-sites
preference. Upgrade cleanup removes retired layout and enabled-sites preferences.
Temporary player state is held in page memory and discarded
as the page or viewing session ends. You can change preferences in the FrameFit menu,
restrict site access in Chrome, or disable or uninstall FrameFit at any time.

## Limited use

FrameFit uses locally processed information only to provide its video-viewing,
per-site preference, and restoration features. It does not transfer that information
for unrelated purposes or allow the developer to inspect it remotely. These practices
comply with the Chrome Web Store User Data Policy, including its
Limited Use requirements.

## Changes and contact

Updates to data-handling practices will be reflected here and in the store disclosures.
For privacy questions, use the project's
[public support page](https://github.com/band-band/framefit-privacy/issues). Do not include
passwords, private browsing details, or other sensitive information in a public issue.

The close-confirmation and hide-compact-tip preferences are also stored locally.
They are not transmitted to the developer or third parties.
