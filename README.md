# Reminders

The Reminders plugin owns Apple Reminders operations for the user's agents.
It uses the external `remindctl` CLI for public EventKit functionality and
AppleScript Accessibility UI scripting for native fields that EventKit omits,
including tags and custom Smart Lists.

The UI path is deterministic macOS automation, not model-driven Computer Use.
It still controls the visible Reminders app, so callers preserve focus, avoid
coordinate clicks, and verify the saved result from the UI-capable surface.

## Retired native app

The deprecated Reminders Clipboard macOS app and its login item were retired on
2026-08-25. This repository now ships only the useful agent plugin. Removing the
app does not delete or modify any Apple Reminders data.
