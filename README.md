# patch notes sync system

this repository exists for one purpose:
**to store and synchronize patch notes for my roblox games.**
it might sound funny, but it’s actually a super convenient way to keep every experience perfectly in sync!

---
## ❓ how does it work?

**a custom discord bot handles the whole pipeline:**

1. when a game’s **place id** is mentioned in my server's `#changelogs` channel,
   the bot detects it.
2. the bot converts the provided **markdown** into **roblox richtext**
3. it appends the formatted patch notes to the correct file in this repo.
4. on roblox, the game reads the **raw file** via an http request.
5. the client displays both current and past patch notes forever.

---

## ❓ why not upload the patch notes here first and have the discord bot publish them?

honestly?
i didn’t think of doing it that way at first 😭.

but this order **does** have some upsides:

* friends and collaborators who don’t use github (or are on mobile) can publish notes easily.
* the bot only needs to convert the notes **once** (to richtext), instead of formatting separately for both discord and roblox.
* it keeps the workflow lightweight and discord-friendly.

if i were to rebuild this system, i’d probably flip the process -
upload the notes directly to github and let both roblox and discord read from here using http and bot mirroring.

but for now?
this setup works great and keeps everything in sync.
