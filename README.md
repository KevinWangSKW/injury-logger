# Injury Logger

A personal injury and pain tracker. Everything you log stays on your own
device — nothing is sent anywhere.

## Body map (3D)
Open the app to a real, rotatable 3D body — drag to turn it, tap a spot to
log something there.
- If nothing's tracked at that spot yet, you'll get a form: what happened,
  the date, how much it hurts right now (0–10), and optional notes. Saving
  it creates a new injury record.
- If something's already tracked there, you'll be asked whether this is a
  new instance of that same injury (a flare-up) or a separate new injury.
- Colored spheres on the model mark everywhere you have something tracked,
  colored by status: red (active), amber (recovering), purple (recurring),
  grey (resolved).

The 3D model is a first-pass approximation matched to the real mesh's
proportions — tap positions are close but not laser-precise at every
boundary; that's expected and fine to live with for now.

## Injuries tab
Every injury you've logged, grouped by status. Tap one to open it:
- **Timeline** — every instance logged, with pain level and notes. Delete
  a single wrong entry without touching the rest.
- **Diagnosis** — empty until you've seen a doctor. Only then does a short
  reference list appear, framed as "what did your doctor diagnose," never
  the app guessing.
- **Rehab plan** — type in exactly what your doctor or PT told you. The
  app never invents or suggests a plan.

Change status, or delete the whole record, from the top of this screen.
You can also dictate into any text field using the 🎤 button.

## Report tab
Filter by body region or diagnosis, see a summary + full timeline per
injury, and print or save as PDF to bring to a doctor's visit.

## Reminders tab
A checklist for today only, pulled from active/recovering injuries' rehab
plans. Resets automatically the next day.

## Where your data lives
Stored in the browser's local storage on the device you're using. Doesn't
sync between devices; cleared if you clear that browser's site data.

## Files in this folder
- `index.html` — the whole app
- `manifest.json`, `sw.js` — installable/offline support
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png` — app icons
- `body-model.glb` — the 3D body model (required for the body map to load)

## Editing it later
Everything's in `index.html`. Open it in a text editor, change it,
re-upload — no build step.

## Credit
3D model: "Human Body Base Mesh Male" (https://skfb.ly/pzC6D) by
ferrumiron6, licensed under Creative Commons Attribution
(https://creativecommons.org/licenses/by/4.0/).
