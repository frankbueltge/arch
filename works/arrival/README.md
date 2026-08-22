# Arrival

A work candidate. Iteration 1, built 2026-08-23 (session 11).

This file is for continuing the work, not for explaining it. The work is the
HTML file; if it needs this README to be understood, it has failed its own
test (`material/operative-model.md`, I5/I6), and that failure belongs in the
record, not in a longer README.

## Rebuilding

    python3 build.py                 # most recent event carrying both products
    python3 build.py us6000tmta      # a named event

Standard library only, Python 3.9+. `build.py` writes `<eventid>.html` next to
itself from `template.html`. Each build is a new instance from live public
data, not a re-render of stored output; the built file embeds its data and its
source URLs and makes no network request when opened.

Requirements on an event: it must carry both a `phase-data` product (the
instrument arrivals) and a `dyfi` product (the human reports). Not every event
has both — `build.py` with no argument walks recent M≥5 events until it finds
one that does.

## Built instances

- `us6000tmta.html` — M 5.8, 4 km N of Toride, Japan, 2026-08-22T17:00:39.472Z.
  123 seismometers, 1.63°–98.04°; 97 human reports in 86 blocks, out to 261 km.

## Provenance and reuse

Data: USGS Earthquake Hazards Program, public and unauthenticated
(`ledger/2026-08-23-session-11-two-perceptions.md` records what was requested
and what came back). Station arrival instants and epicentral distances are
taken as published in the QuakeML; travel time is the only derived quantity
(pick instant minus origin instant) and 1° is taken as 111.195 km along the
surface. Nothing is smoothed, fitted or interpolated — every mark is one
published measurement.
