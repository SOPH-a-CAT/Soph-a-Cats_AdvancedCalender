# Daydream — Soph-a-Cat's Advanced Calendar

**[Open the calendar website](https://soph-a-cat.github.io/Soph-a-Cats_AdvancedCalender/)**

A colorful monthly calendar built with plain HTML, CSS, and JavaScript. No frameworks or external libraries.

## Features

- Pastel weekday columns and daily scheduled-time fill
- One-time or weekly events, with start/end times and optional locations
- Weekly repetition forever or through the event's month
- Browser-local saved schedules
- Share URLs with Show or Personal privacy choices; Personal removes original titles and locations before encoding
- Read-only shared calendars with a time-zone label and an all-dates event sidebar

## Run locally

Serve the `dist` directory with any static web server. For example:

```sh
python3 -m http.server 8000 --directory dist
```

Then open http://localhost:8000. Deploy `dist` to any static website host.

## Tests

With Node.js installed:

```sh
node tests/sharing.test.cjs
node tests/share-flow.test.cjs
```

## Storage and sharing

Events stay in the browser's local storage and do not sync between devices. Share URLs contain a snapshot of selected event details, dates, times, and recurrence rules. Anyone with a link can read or forward its contents. Existing links do not update or expire when the original calendar changes. Shared times remain in the calendar's labeled time zone.

This repository contains application source and synthetic tests, not personal calendar records or hosting credentials.
