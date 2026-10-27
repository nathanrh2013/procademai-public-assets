# Procademai — Public Assets

The **single master host** for publicly linkable Procademai files (campaign social visuals, etc.).
Everything public lives here, organized per campaign, so there is one predictable place to look —
and one clear boundary for what is allowed to be public.

Files are served to tools (Buffer, etc.) via GitHub raw URLs.

## IP boundary (read before committing)

Only **non-sensitive, publish-ready, already-public-facing** assets belong here — e.g. the social
graphics that publish to LinkedIn anyway. Everything committed here is **world-readable, forever.**

Do **not** put here: internal methodology, the NxT operating-model core, source/design files,
drafts, data, source registers, or anything behind the NDA / IP line. When in doubt, keep it out.

## Structure (per campaign)

```
campaigns/<campaign-code>/<asset files>
```

`<campaign-code>` matches the Holman OS GTM calendar code — series + sequence + year-month,
lowercased. Example: NxT November 2026 = `ngo-01-2026-11`.

## Raw URL pattern

```
https://raw.githubusercontent.com/nathanrh2013/procademai-public-assets/main/campaigns/<campaign-code>/<filename>
```

## Campaign index

| Campaign | Code | Folder | Contents |
|---|---|---|---|
| NxT — Next Gen Procurement Organization (Nov 2026) | NGO-01 | `campaigns/ngo-01-2026-11/` | Day01–Day30 post lead visuals (1080×1350 PNG) |
| Procademai — Procurement AI Value Diagnostic (Nov 2026) | ASP-01 | `campaigns/asp-01-2026-11/` | 27 of 32 November LinkedIn post lead visuals (1080×1350 JPG) — the final, uploaded D-019 graphic for each post that has one; filenames are `<label>_<Holman-OS-post-id>.jpg` so each maps 1:1 to its Buffer draft and its row in `calendar-data.json`. 5 posts (Nov 1 AIE look-ahead, Nov 5, Nov 12, Nov 19, Nov 30 AIE look-back) have no final graphic yet and are not here. |

---
© 2026 Procademai / Holman & Holman LLC
