# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Messaging / Media Paths

- For sending files back to chat with `message.send`, stage/copy files into:
  - `/home/labs/.openclaw/media/outbound/`
- Files under workspace (e.g. `/home/labs/.openclaw/workspace/...`) may be blocked by provider path allowlists.
- Default send flow:
  1. Generate file in workspace (or anywhere)
  2. Copy to `/home/labs/.openclaw/media/outbound/`
  3. Send using `message` tool with `filePath` from outbound path

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.
