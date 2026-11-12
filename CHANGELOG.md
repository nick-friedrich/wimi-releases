# Changelog

Downloads for every version are on the [Releases](https://github.com/nick-friedrich/wimi-releases/releases) page.

## 1.1.0

Design your own layouts, keep windows clear of third-party docks, and find out when another app is using Wimi's shortcuts too.

### New
- Custom layouts (Pro): make your own layout from up to four columns of one to three stacked windows, and drag its dividers to set the sizes. Start from the New Layout card in Layouts, right-click a layout to edit or copy it, or click Save as Layout to keep the shape you've dragged your windows into. Custom layouts work in search, the workspace bar menu and Next / Previous layout.

### Improved
- Screen margins: in Settings → Windows, set how much space layouts leave free at the top, bottom, left and right of each display, so windows stay clear of third-party docks such as DockDoor or other bars that cover them.
- When another app, such as Raycast or Rectangle, reacts to one of Wimi's shortcuts and moves your windows too, Wimi now tells you once and names the window managers that are running, so you can remove the duplicate shortcut.

### Fixes
- A window too big for its slot no longer trades places with its neighbor when you focus it with Hyper + arrow keys.
- Temporary license-server errors, rate limits and firewall responses no longer remove an activated license. Failed deactivation keeps the license and activation ID so you can retry.
- Turning on Hyper no longer erases other key remappings, such as `hidutil` remaps or macOS's per-keyboard modifier key settings. Turning it off or quitting restores the previous Caps Lock mapping.
- Entering a license key for a different product no longer uses up one of that key's activations.
- Unplugging an external keyboard no longer releases Hyper or modifiers you're holding on another keyboard.

## 1.0.2

Layouts that leave your windows usable: they get their size back when they leave a layout, and apps that can't shrink to fit no longer push their neighbors off screen.

### New
- Reset a layout's window sizes, for example to get 2/3 – 1/3 back after dragging it to halves: choose the active layout again (click it, pick it from the workspace bar or press its shortcut), press Hyper 0 (⌃⌥⌘0), or search "Reset layout sizes". Change the key in Settings → Shortcuts.
- New setting in Settings → Windows, "Put windows back when quitting Wimi": tiled windows return to where they were before Wimi arranged them.
- What's New… in the menu bar menu opens the changelog at getwimi.app/changelog, in case you closed the update notes too quickly.

### Improved
- Apps that can't get as small as their slot (Notion, Xcode) now overlap the window next to them instead of squeezing it or pushing it off screen, so every window stays usable. The window you're using stays on top; click the other to bring it forward. A warning sign in the workspace bar, the window switcher and the Layouts view says which app needs more room.
- Turning a layout off puts every window back where it was before Wimi tiled it, not just the hidden ones.
- With "Moving a window yourself: Takes it out of the layout", dragging a window out of its slot gives it back its original size.

## 1.0.1

Fixes for setups with several displays, and faster workspace switches.

### Improved
- Switching workspaces starts about twice as fast, and windows of apps with windows in both workspaces (Safari, Finder) no longer pause mid-slide.
- The first time Wimi hides a window, it offers once to open Desktop & Dock settings if "Group windows by application" is off, which keeps Mission Control readable.

### Fixes
- Hidden windows no longer stay visible or move to another workspace when a display's bottom corners are blocked by its neighbors, as can happen with three monitors or a laptop above a wider display.
- Dragging a tiled window to a display without a layout gives it back the size it had before the layout.
- Dragging a staged window to a smaller display no longer snaps it back or shrinks your saved staged size.
- Windows that Wimi places freely (dragged to a display without a layout, or popped out) no longer cover the workspace bar.
- Windows waiting behind a layout in another workspace stay in that workspace when a display disconnects.
- Switching workspaces tries again if a busy app missed the move, so its window doesn't stay hidden.

## 1.0.0

Wimi 1.0: free to use, with Wimi Pro for the power features. Everyone gets 30 days of Pro to try it, and for six weeks Pro is half price.

### Free and Pro
Wimi stays free: the drawer, the window switcher with live previews and ⌥Tab, search, the app launcher, emoji, Keep Awake, the Hyper key, and the Fullscreen, Staged and Halves layouts.

**Wimi Pro** adds:
- **Advanced layouts:** thirds, quarters, 2/3–1/3, stacked and main+side.
- **Staged window size:** size the staged window with a slider in the Layouts drawer or by dragging its edges. Each display and workspace keeps its own size. This replaces the Small/Medium/Large setting.
- **Workspaces** and the **workspace bar**, including the workspace number in the menu bar.
- **The always-visible strip.**
- **Clipboard history.**
- **Glass themes:** Glass, Liquid Glass, Sheet and Midnight.

Pro is **$19.99 once** (plus tax): no subscription, and your key works on two Macs. **Launch offer: $9.99 with the code LAUNCH50 until December 22.** Buy it from Settings → License, where you also enter your key.

**Updating from a beta?** Thank you for testing! Everything stays unlocked for 30 days from this update. After that, Wimi keeps working on the free plan, and your Pro settings (layouts, workspaces, the bar, your theme) wait for you until you buy. Nothing is deleted.

### New
- **Settings → License:** see your trial, buy Pro and enter your key. The sparkle button above Settings in the drawer takes you there.
- **Settings → Feedback:** email us from your mail app (or copy the address) or report a bug on GitHub.
- With all workspaces shown, the window switcher can list windows most recently used first instead of grouped by workspace ("Group by workspace" in the drawer footer and Settings → Windows). The workspace bar keeps its grouping.
- The welcome tour ends with a page about Wimi Pro and where your trial stands.

### Improved
- The drawer can reopen on the tab you left it on: Settings → General → Open in → Last used tab. Scrolling over the drawer's tab bar switches tabs.
- The drawer's see-through backgrounds (Transparency, Sheet, Glass, Liquid Glass) have a half-transparent wash behind the content, so text stays readable over a bright desktop.
- Wimi sends one anonymous event when your trial starts, so we know how many people try it: the event and the Wimi version, nothing else. Turn it off on the welcome screen or in Settings → General → Privacy.

### Fixes
- Steam's windows show up in the window switcher and join layouts. Steam draws them from a helper process with its own title bar, which Wimi used to skip.
- ⌘Tab or a Dock click to Finder switches to the workspace holding its window, like every other app. Clicking the desktop still doesn't switch.

## 0.5.0

### New
- **Top and bottom (experimental):** the drawer can open from the top or bottom edge, handy as an app launcher. The always-visible strip follows it and stacks with the workspace bar.
- **Clock and calendar:** an optional clock in the workspace bar; click it for a month calendar. Settings → General → Clock & Calendar.
- **Calendar in the drawer:** a Calendar mode with week numbers and optional calendar events.
- **Reorder the workspace bar** by dragging its windows, also into another workspace's group.
- **Collapse the workspace numbers** to the ones with windows.

## 0.4.0

### New
- **Workspaces (early):** Hyper 1–9 switches between nine workspaces, Hyper ⇧1–9 sends the focused window to one. Each workspace keeps its own windows and its own layout on each display; search finds windows in all of them.
- **Workspace bar (optional):** a bar at the top or bottom of every display with the workspaces, that display's windows and a layout menu. Drag a window's icon onto a workspace number to send it there.
- **Strip on every display:** Settings → General → Bar display → All displays gives each display its own always-visible strip with just that display's windows.
- **Floating apps:** choose apps in Settings → Windows whose windows stay out of layouts.
- **New backgrounds:** Midnight and Liquid Glass (macOS 26 and later). Settings → General → Theme.

### Improved
- The drawer has a roomier look: corners that match your windows, more padding, bigger search results and clipboard cards.
- The always-visible strip and workspace bar use much less CPU.
- The emoji picker shows six bigger emoji per row.

### Fixed
- The welcome window comes back at the step you were on when macOS reopens Wimi after granting a permission.
- Show desktop also clears Finder's windows and no longer leaves apps hidden.
- Unhiding an app no longer brings back windows a layout had parked.
- Dialog sheets that would hang off the screen now fit.

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
