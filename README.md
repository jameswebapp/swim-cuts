# 🏊 Swim Cuts — Time Standards Ladder

**See where your kid's time lands** — one ladder from B to the Olympic Trials:
Motivational levels, Maryland LSC championships, Eastern Zone meets, NCSA,
Futures, Juniors, U.S. Nationals / U.S. Open, and the 2028 Olympic Trials
standards, all merged and sorted by time.

### ▶ Use it [now](https://jameswebapp.github.io/swim-cuts/)

No account, no install, works offline after the first visit. Times you enter
stay on your device (localStorage) — nothing is uploaded.

## Who it's for

- **Swim parents** — your kid just swam a time at a meet and you want to know,
  right there on deck: *what cut is that, and what's next?*
- **Age-group & high-school swimmers (about 10–18)** — Motivational B → AAAA,
  LSC and Zone championships, NCSA, Futures and Junior Nationals on one ladder.
- **College-age and senior swimmers (up to 22 and beyond)** — the Open tier:
  EZ Sectionals, U.S. Nationals, the U.S. Open, and the 2028 Olympic Trials
  standards at the top of the ladder.
- **Coaches** — a 5-second sanity check instead of flipping through six PDFs.

## How to use

1. Pick gender, age (age on the first day of the meet), course (SCY / SCM / LCM),
   stroke and distance.
2. Tap the big time and just type digits — `2850` becomes `28.50`,
   `12667` becomes `1:26.67`.
3. The ladder shows every standard for that event: the highest cut you made,
   the next cut and exactly how many seconds away it is.
4. Add times to the session list and sort by level, or by "closest to next cut".

**On your phone:** open the link, then
- iPhone (Safari): Share → *Add to Home Screen*
- Android (Chrome): ⋮ menu → *Install app* / *Add to Home screen*

It then behaves like a native app — full screen and offline at the pool deck.

## What's inside (9,908 standards)

| Set | Edition |
|---|---|
| USA Swimming Motivational (age-group + single-age) | 2024–2028, Oct 2025 revision |
| Maryland LSC Champs / Jr Champs (SCY & LCM) | 2026 |
| Eastern Zone Age Group Champs (SC & LC) / Sectionals | 2026 |
| NCSA Age Group / NCSA Juniors (Spring & Summer) | 2026 (Age Group unchanged for 2027) |
| Futures · Winter Juniors · Summer Juniors | 2026 |
| U.S. Nationals (18&U and 19&Over tables) / U.S. Open | 2026 |
| U.S. Olympic Team Trials (LCM only, as published) | 2028 |

Every set is sourced from its official document — see the **References** tab
inside the app for the full list with links. Standards that were never
published are never shown (no estimates, no conversions).

Notes:
- **MD Jr Champs** is a *band*, not a floor: your time must be slower than the
  MD Champs cut and at or under the Jr Champs bound shown in the ladder.
- Each meet shows the edition closest to today going forward: if the next
  edition's standards aren't published yet, the most recent one is used.

## References

Every standard comes from its official document (the app's References tab has
the same list):

- **Motivational (Age Group + Single Age)** — [USA Swimming official standards page](https://www.usaswimming.org/times/time-standards) · [SCY standards PDF](https://www.gomotionapp.com/catcc/UserFiles/Image/QuickUpload/2028-usa-motivational-scy_080685.pdf) · [SwimStandards cross-check](https://swimstandards.com/national/quad)
- **MD Champs / MD Jr Champs** — [SCY Champs standards](http://www.opsthammerheads.org/recdsaopst/UserFiles/Image/QuickUpload/2025---2026-mdlsc-scy-championship-meet-qualifyingtimes-sr-champs-14-u-champs-1--007673_052207.pdf) · [LCM standards](https://www.gomotionapp.com/md/UserFiles/Image/QuickUpload/2026-long-course-cut-times-1-_091328.pdf) · [Jr Champs / LCQ document](https://www.gomotionapp.com/md/UserFiles/Image/QuickUpload/lcq-2026---final_023418.pdf)
- **EZ Age Group Champs (SC / LC)** — [Short-course meet announcement](https://www.ctswim.org/Customer-Content/www/Meets/SC2025-26/March/2026-eastern-zone-age-group-championships-meet-announcement_060363.pdf) · [Long-course meet announcement](https://www.ctswim.org/Customer-Content/www/CMS/files/meets/2026_LC_Meets/2026_EZ_LC_Age_Group_Champs_FINAL_updated.pdf)
- **EZ Sectionals** — [Official standards PDF](https://www.niagaraswim.org/eznslsc/UserFiles/Image/QuickUpload/speedo-sectional-qualifying-times-2026_000714.pdf)
- **NCSA Age Group** — [Standards PDF](https://www.hinsdaleswimming.org/ishsc/UserFiles/Image/QuickUpload/2025-26-ncsa-spring-age-group-championships-time-standards_021639.pdf) · [SwimStandards cross-check](https://swimstandards.com/ncsa/age-group-times)
- **NCSA Juniors (Spring / Summer)** — [Spring standards PDF](https://www.memphistigerswimming.com/semts/UserFiles/Image/QuickUpload/2026-ncsa-jr-time-standards_049965.pdf) · [Summer meet announcement PDF](https://swimstandards.com/data/2026-ncsa-summer-championship-meet-announcement-sanctioned_081104.pdf)
- **Futures** — [Official standards PDF](https://www.swimspa.org/stspa/UserFiles/Image/QuickUpload/futures-time-standards_014128.pdf)
- **Winter Juniors** — [USA Swimming official standards page (2026 standards documents)](https://www.usaswimming.org/times/time-standards)
- **Summer Juniors** — [Official standards PDF](https://irp.cdn-website.com/4e47d36a/files/uploaded/2026+Speedo+Junior+National+Championships_Time+Standards.pdf)
- **U.S. Nationals** — [Official standards PDF](https://websiteprodcoresa.blob.core.windows.net/sitefinity/docs/default-source/timesdocuments/time-standards/2026/18077640025_events_2026_toyotanationalchampionships_timestandards.pdf?sfvrsn=c071832_3)
- **U.S. Open** — [Official standards PDF](https://usaswimming.org/docs/default-source/timesdocuments/time-standards/2026/timestandards_2026_toyotausopen082826.pdf?sfvrsn=5381e32_7)
- **Olympic Trials** — [Official standards PDF](http://www.usaswimming.org/docs/default-source/timesdocuments/time-standards/2028/2028_olympictrials_timestandards.pdf) · [USA Swimming announcement](https://www.usaswimming.org/news/2026/10/15/usa-swimming-announces-qualifying-standards-for-2028-us-olympic-team-trials-swimming)

## Tech

Fully static PWA — `index.html` + `standards.json` + service worker.
No backend, no build step, no tracking. To update the data, replace
`standards.json` and bump the cache name in `sw.js`.

## Disclaimer

Unofficial reference tool, not affiliated with USA Swimming, Maryland
Swimming, Eastern Zone Swimming, or NCSA. Always confirm qualifying times
and eligibility against the official meet announcement before entering.
