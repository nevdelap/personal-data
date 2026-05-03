# Personal Data

> **Disclaimer for those who have stumbled across this somehow:** This is vibe
> coded — which I define as built in a language I don't know well enough to
> write and debug production code in myself (JavaScript). I can look at it and
> say "Mmm, purdy.", but not a lot else. I use it to store unimportant data.
> Because it stores data you shouldn't use it for anything important, and
> probably shouldn't use it at all. The repository is public only so I can
> publish it via GitHub Pages for my own use — it is not intended for anyone
> else.

A configurable personal data tracker. Log metrics like blood pressure, weight,
and anything else you want to track — stored in Firebase, accessible from any
device.

## Features

- **Configurable fields** — define what you want to track, with optional notes
  per field shown as hints in the entry form
- **Draggable field order** — reorder fields by dragging in the setup screen
- **Timestamped entries** — log with the current time, or edit it to backfill
  past readings
- **Cloud storage** — data is stored in Firebase Realtime Database and accessible
  from any device
- **Private by key** — your data is stored under your personal key; only
  someone with your Firebase credentials and personal key can access it
- **Delete with undo** — delete entries with a 5-second undo toast
- **Light and dark modes** — follows your system preference, or can be set
  manually

## Setup

1. Create a [Firebase](https://console.firebase.google.com) project and enable
   Realtime Database
2. Open the app and enter your Firebase API key, database URL, and a personal
   key of your choosing
3. Define the fields you want to track

Your password manager will save the database URL as the username and the API
key as the password, so both are filled automatically on return visits. The
personal key is not saved by the password manager — pick something short and
memorable. You can use different personal keys to store separate sets of data
in the same Firebase database.

Credentials are stored only in the browser's local storage — nothing is
hardcoded.

## License

- App code: [MIT](LICENSE)

## Local development

```bash
just serve    # serve locally and open in browser
just format   # format Markdown
just lint     # format then lint
```
