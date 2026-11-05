# Investeerimiskonsultant — Claude'i püsijuhis

See repo on Remy (Richard) Lightyeari IK portfelli otsustussüsteem. **Iga sessioon selles repos töötab PIIBLI järgi.**

@PIIBEL.md

## Alati, iga sessiooni alguses
1. Loe `PIIBEL.md` (reeglistik — kõrgeim prioriteet) ja `claude/OTSUSED.md` (§18).
2. Loe `portfell/SEIS.md` — viimane teadaolev portfelli seis ja watchlist.
3. Tänane kuupäev + nädalapäev + kellaaeg Tallinna aja järgi (§15.12).

## Konfliktid
- **PIIBEL (kehtiv versioon PIIBEL.md päises) on ülim.** Kui mõni oskus (skill), nt `portfelli-analuus` (vana 50/30/10/10 strateegia), või vanem mälu on PIIBLIGA vastuolus, kehtib PIIBEL. Ütle vastuolu välja.
- PIIBLIT muudetakse ainult Remy loal. Muudatus = uus versiooninumber + kanne §16, kui põhjuseks oli viga.

## Failid
| Fail | Sisu | Kes muudab |
|---|---|---|
| `PIIBEL.md` | Reeglistik | Ainult Remy loal |
| `claude/OTSUSED.md` | ❓ ootab otsust · ✅ sinu teha · 📅 kalender · päevik (§13, §18) | Claude |
| `portfell/SEIS.md` | Positsioonid, kaalud, sularaha, watchlist, 2035 laused, falsifikatsioonid | Claude (Remy ekraanipiltide põhjal) |
| `analuusid/AAAA-KK-PP.md` | Päeva-/täisanalüüsid (detailid) | Claude |

## Ajastatud analüüs (autonoomne)
Ajastatud käivitus ei näe Lightyeari kontot. Ta töötab `portfell/SEIS.md` viimase seisu pealt ja märgib selle kuupäeva. Kui seis on >14 päeva vana, lisab ❓ alla palve saata uued ekraanipildid. Ajastatud käivitus **ei tee ega kinnita kunagi tehinguid** — ainult analüüs, lipud ja mustandid Remy kinnitamiseks (§18.3).

## Git
Pärast iga analüüsi: commit + push (failid peavad püsima, konteiner on ajutine). Commit-sõnum eesti keeles, nt `Analüüs 2026-11-06 (R)`.
