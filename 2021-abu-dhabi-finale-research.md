# 2021 Formula 1 Season Finale — Abu Dhabi Grand Prix Research Brief

Retrospective research trail for the racing newsletter. All data points below are reported exactly as returned by the F1 data source lookups.

## 1. Race Session Identification

| Field | Value as reported |
|---|---|
| Race | 2021 Abu Dhabi Grand Prix (Season 2021, Round 22) |
| Venue | Yas Marina Circuit — Abu Dhabi, UAE (lat 24.4672, long 54.6031) |
| Date | `2021-12-12` (race start `13:00:00Z`) |
| Session key | **Not returned by the session database.** The `getHistoricalSessions` endpoint returned no record for the 2021 Yas Marina race — queried with year 2021, circuit short names `yas_marina` / `Yas Marina Circuit` / `Yas Marina`, location `Abu Dhabi` / `Yas Island` / `Yas Marina`, country `UAE` / `United Arab Emirates`, and session name `Race`, plus a cache clear — all returned empty. As a control, the same endpoint was queried for other 2021 circuits (Monza, Spa) and for 2023 Abu Dhabi with the same filters; all also returned empty, so the session database's coverage for these events is not exposed through this endpoint. The race date above is reported exactly as returned by the historical race results source for Season 2021 / Round 22. |

## 2. Classified Race Results — 2021 Abu Dhabi Grand Prix (Season 2021, Round 22)

| Pos | Driver | Car # | Constructor | Grid | Laps | Status | Time / Gap | Pts |
|-----|--------|-------|-------------|------|------|--------|------------|-----|
| 1 | Max Verstappen | 33 | Red Bull | 1 | 58 | Finished | 1:30:17.345 | 26 |
| 2 | Lewis Hamilton | 44 | Mercedes | 2 | 58 | Finished | +2.256 | 18 |
| 3 | Carlos Sainz | 55 | Ferrari | 5 | 58 | Finished | +5.173 | 15 |
| 4 | Yuki Tsunoda | 22 | AlphaTauri | 8 | 58 | Finished | +5.692 | 12 |
| 5 | Pierre Gasly | 10 | AlphaTauri | 12 | 58 | Finished | +6.531 | 10 |
| 6 | Valtteri Bottas | 77 | Mercedes | 6 | 58 | Finished | +7.463 | 8 |
| 7 | Lando Norris | 4 | McLaren | 3 | 58 | Finished | +59.200 | 6 |
| 8 | Fernando Alonso | 14 | Alpine F1 Team | 11 | 58 | Finished | +1:01.708 | 4 |
| 9 | Esteban Ocon | 31 | Alpine F1 Team | 9 | 58 | Finished | +1:04.026 | 2 |
| 10 | Charles Leclerc | 16 | Ferrari | 7 | 58 | Finished | +1:06.057 | 1 |
| 11 | Sebastian Vettel | 5 | Aston Martin | 15 | 58 | Finished | +1:07.527 | 0 |
| 12 | Daniel Ricciardo | 3 | McLaren | 10 | 57 | +1 Lap | — | 0 |

**Fastest lap:** Max Verstappen, lap 39 — 1:26.103 (220.800 kph), rank 1.

**Podium in finishing order:**
1. **Max Verstappen** (Red Bull, 33)
2. **Lewis Hamilton** (Mercedes, 44)
3. **Carlos Sainz** (Ferrari, 55)

## 3. Podium Driver Profiles (as reported by the profile lookup)

### Lewis Hamilton (P2)
- Permanent number: 44
- Three-letter code: HAM
- Nationality: British
- Date of birth: 1985-01-07
- Profile link: http://en.wikipedia.org/wiki/Lewis_Hamilton

### Max Verstappen (P1)
- Permanent number: 3
- Three-letter code: VER
- Nationality: Dutch
- Date of birth: 1997-09-30
- Profile link: http://en.wikipedia.org/wiki/Max_Verstappen

### Carlos Sainz (P3)
- Permanent number: 55
- Three-letter code: SAI
- Nationality: Spanish
- Date of birth: 1994-09-01
- Profile link: http://en.wikipedia.org/wiki/Carlos_Sainz_Jr.

## 4. Championship Context

Verstappen and Hamilton arrived at the finale level on points (369.5 each before the round). Final 2021 standings after Round 22: Verstappen 395.5 (champion), Hamilton 387.5, Bottas 226, Pérez 190, Sainz 164.5. Verstappen's win, decided on the final lap of the last-lap restart, secured his first Drivers' Championship.

## 5. Sources

- Historical race results: Season 2021, Round 22 (2021 Abu Dhabi Grand Prix)
- Driver profile lookups: `hamilton`, `max_verstappen`, `sainz`
- Historical sessions database (queried; no 2021 Yas Marina session record returned)