# Injury Logger

A personal injury and pain tracker. Everything you log stays on your own
device — nothing is sent anywhere.

## Body map
Open the app to a front/back diagram of a body. Tap a spot to log something
there.
- If nothing's tracked at that spot yet, you'll get a form: what happened,
  the date, how much it hurts right now (0–10), and optional notes. Saving
  it creates a new injury record.
- If something's already tracked there, you'll be asked whether this is a
  new instance of that same injury (a flare-up) or a separate new injury.
  Keeping flare-ups attached to one record instead of creating duplicates
  is what keeps your history readable later.

Dots on the diagram are colored by status: red (active), amber (recovering),
purple (recurring), grey (resolved).

## Injuries tab
Every injury you've logged, grouped by status. Tap one to open it:

- **Timeline** — every instance logged for that injury, with pain level and
  notes. You can delete a single wrong entry here without touching the rest.
- **Diagnosis** — empty until you've actually seen a doctor. When you add
  one, you'll see a short reference list of common diagnoses for that body
  area to pick from (or you can type your own) — this only records what a
  doctor told you, it is never the app guessing what you might have.
- **Rehab plan** — where you type in the exact plan your doctor or physical
  therapist gave you (exercises, sets/reps, frequency, restrictions). The
  app never invents or suggests a plan itself.

You can also change an injury's status (active / recovering / resolved /
recurring) at the top, or delete the whole record with "Delete record."

## Reminders tab
A checklist for **today only**, pulled from the rehab plans of any injury
currently marked active or recovering. Check an exercise off once you've
done it; the checkmarks reset automatically the next day. This tab doesn't
send you notifications — you need to open the app to see it.

## Where your data lives
Everything is stored in the browser's local storage on the device you're
using. It doesn't sync between your phone and a computer, and it will be
erased if you clear that browser's site data. If you switch devices, your
history won't carry over automatically.

## Editing the app itself
Everything is in the one `index.html` file. Open it in a text editor (or
edit it directly on GitHub), make your change, and re-upload — no build
step needed.
