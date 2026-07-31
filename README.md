# Kestrel — Support & Issue Tracker

Public bug reports and feature requests for **Kestrel**, a premium watch face for Garmin
Connect IQ devices.

> This repository contains **no source code** — it exists purely so that issues and requests
> are tracked somewhere public, searchable, and out in the open.

## I found a bug

**[→ Report a bug](../../issues/new?template=bug_report.yml)**

Please include your **exact watch model** and **firmware version** (on the watch:
`Settings → System → About`). Most rendering issues are specific to one screen size or
firmware, so without the model a report usually can't be acted on.

## I have a feature request

**[→ Request a feature](../../issues/new?template=feature_request.yml)**

Before opening one, please [search existing issues](../../issues?q=is%3Aissue) — if the
request already exists, a 👍 on it is more useful than a duplicate, because reactions are
what get sorted by.

## Before you file

A few things that are already known, so you don't spend time writing them up:

| Symptom | Explanation |
| --- | --- |
| A metric shows `--` or is blank | Kestrel only displays what your watch actually records. Values like VO₂ Max or Body Battery appear only once your watch has computed them. |
| Resting heart rate looks "wrong" | It's Garmin's own **7-day average** resting HR from your user profile, not last night's low. |
| Sleep score isn't available as a metric | Connect IQ exposes no sleep score to watch faces on any current device. It isn't something a watch face can read. |
| Always-on display looks dimmer / shows less | Required. Garmin caps how many pixels a face may light in always-on mode to protect AMOLED screens from burn-in. |
| Numbers use a different font than the clock | Some models don't ship the font family the clock uses, so values fall back to a different one. Tracked. |

## Roadmap & status

Issue labels tell you where something stands:

- `status: confirmed` — reproduced, queued for a fix
- `status: needs info` — waiting on details (usually watch model or firmware)
- `status: planned` — accepted, will be built
- `status: shipped` — released; the issue notes which version
- `status: not possible` — blocked by a Connect IQ platform limit, with the reason

## Links

- **Get Kestrel** — search **Kestrel** in the Garmin Connect IQ Store app, or on
  [apps.garmin.com](https://apps.garmin.com)
- **Privacy policy** — https://nav1885.github.io/app-policies/kestrel/privacy.html
- **Email** — nhc002@gmail.com

## Supported devices

Kestrel targets **54 Garmin models** across 7 display classes (240–454 px, MIP and AMOLED),
including the fēnix 7/8 families, epix and epix Pro, Forerunner 165/170/255/265/570/955/965/970,
Venu 2/3/4, Vívoactive 5/6, Instinct 3 AMOLED, MARQ Gen 2, Enduro 3, and the
Descent/Approach/D2/tactix/quatix variants that share those screens.

If your watch isn't listed in the store as compatible, open a **feature request** naming the
model — device support is usually straightforward to add when the screen size is one already
handled.
