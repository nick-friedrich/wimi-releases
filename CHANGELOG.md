# Changelog

Downloads for every version are on the [Releases](https://github.com/nick-friedrich/wimi-releases/releases) page.

## 0.3.1

### New
- The menu bar menu has **Get Launch Discount…** (join the 1.0 launch list for 50% off) and **Send Feedback…**.

### Fixed
- **Show desktop** brings back every window you could see (all windows of a split layout), not just the front one.
- The **Hyper key** no longer fails silently on external keyboards without Input Monitoring access: Wimi asks for it, and Settings shows a warning with a link to grant it.

## 0.3.0

### New
- **Automatic updates:** Wimi checks for new versions once a day and offers to install them. Turn it off or check by hand in Settings → General, or use Check for Updates… in the menu bar. Coming from 0.2.0 or earlier, install this version manually once.
- **Show desktop:** Hyper D (or the button in the drawer header) hides every app. Press it again to bring back the window you were in.
- **Float / join with one key:** Hyper F floats the focused window out of its layout and puts it back in.
- **Join all:** a button in the Windows drawer and the window strip puts every window into the layout of its screen, including floating ones.
- New app icon and a ribbon menu bar icon.

### Improved
- Layouts mode: pick a layout with the arrow keys.

### Fixed
- Buttons in the drawer show their description on hover.

## 0.2.0

### New
- **Window animations:** windows slide into their layout slots, and windows coming back into a layout enter from the screen edge in front of the one they replace. Turn it off or pick the entry edge in Settings → Layouts. Off automatically with Reduce Motion.
- **Swap windows:** Hyper ⇧ + arrow keys swap the focused window with the window in that direction (1 | 2 → 2 | 1).
- **Rotate windows:** Hyper R rotates every window in the layout one slot on, clockwise; Hyper ⇧R rotates back.
- **Pop out window:** a button on window cards (and an optional shortcut) floats a window out of its layout. **Join layout** brings it back.
- **Suggested shortcuts:** Search, Clipboard, Emoji, Layouts and next / previous layout are bound to Hyper chords by default. Restore them anytime in Settings → Shortcuts.
- Opening the drawer by resting the pointer at the screen edge can be turned off.

### Improved
- Hyper + arrow keys wrap around past the edge of a split layout. In Staged and Fullscreen, ← / → step through the hidden windows, which now slide in on top.
- Apps with a minimum size no longer spill over their neighbor: the divider moves to make room, and the window you're using stays on top if they still can't all fit.
- Clearer explanation of the Hyper key.

### Fixed
- Hyper + arrow keys did nothing on some Macs because Wimi couldn't tell which window was focused.

## 0.1.2

First public release.

- Welcome window on first launch to help set up permissions.
- Reopening Wimi while it is running shows a window, so it can always be found again.
- Clipboard history is opt-in (off by default).
- Layouts: windows move across displays instead of swapping, windows can be released from a layout, and a sidebar **Join layout** action.
