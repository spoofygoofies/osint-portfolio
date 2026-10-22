# Drone strike on a residential building, Kyiv (Desnianskyi district), 7 October 2026
### An open-source collection and verification case

Version 1.0 · 21 October 2026 · Self-directed. All times in UTC (Kyiv = UTC+3).

This case shows how reports and footage of one strike were collected from public Telegram channels with a chain of custody, and how the reported location and casualty figures were checked across sources. The exact building is deliberately not identified (sections 7 and 8).

## 1. Key findings

| Finding | Confidence | Basis |
|---|---|---|
| A drone hit a 12-storey residential building in Kyiv on the evening of 7 October 2026, causing a fire at the 10th-floor level that spread to the upper floors. | High | Mayor, State Emergency Service (DSNS), footage from local media |
| The building is in the Desnianskyi district. | High | Mayor's post and Kyiv24 footage reports; no source supports another district |
| The Kyiv Independent placed the strike in the Darnytskyi district and attributed this to the mayor. This is likely an error. | Moderate | The mayor's own post says Desnianskyi; every collected source that names a district agrees |
| 4 people were injured, including 2 children; 22 were rescued, including 8 children. | High (as officially reported) | DSNS post 76916 |
| 2 people were killed; their bodies were found in one damaged apartment the next morning. | Moderate | Two media channels, one citing DSNS; the DSNS post itself was not collected |
| One later post reported five injured. | Not confirmed | Single source; all others report four |

## 2. Scope and questions

1. What happened, and when was it first reported?
2. Where did it happen, to district level?
3. How many people were affected, according to official sources?
4. Can the public sources be preserved so that someone else can check them later?

Out of scope: identifying the exact building, the people affected, and the type of drone.

## 3. Sources and method

- **Sources monitored:** Mayor Vitali Klitschko's channel, the State Emergency Service (DSNS), and two local media channels, Kyiv Operatyvnyi and Kyiv24. ASTRA and Exilenova+ were searched for night footage of the fire; none was found.
- **Collection:** 10 posts from 4 channels were collected on 19 October 2026 between 17:17 and 18:02 UTC with [tg-evidence-collector](https://github.com/spoofygoofies/tg-evidence-collector) v0.1. The tool saved 41 original media files (35 photos, 6 videos, 448 MB) without re-encoding, computed a SHA-256 hash for each, recorded post, edit and collection times in UTC, saved every post page to the Wayback Machine, and logged each action in an append-only custody log. All 41 hashes are unique and all 10 post pages were archived. The hash list is in [`hashes.csv`](hashes.csv).
- **Verification:** location and casualty claims were compared across sources. Sources that only repeat another source were counted once. Times come from post metadata, not from post text.

| Task | Tool |
|---|---|
| Collection, hashing, archiving | tg-evidence-collector v0.1 (Telethon, Wayback Machine) |
| Notes during monitoring | Manual collection log |
| Street-level imagery | Google Street View (newest imagery in the area: 2015) |
| Maps | Google Maps, OpenStreetMap |

## 4. Timeline (UTC)

| Time (UTC) | Event | Source |
|---|---|---|
| 7 Oct 19:23 | Mayor: after an enemy attack, a fire in a 12-storey residential building in the Desnianskyi district at the 10th-floor level; emergency services on the way | Klitschko, post 7792 |
| 7 Oct 19:24 | Kyiv Operatyvnyi repeats the mayor's text, with a photo | Kyiv Operatyvnyi, 198147 |
| 7 Oct 21:01 | DSNS: a Russian drone hit the building at the 10th-floor level; fire spread to the upper floors; partial collapse of structures; 22 rescued (8 children), 4 injured (2 children); fire of 100 m² put out. The district is not named. **The post was edited on 8 Oct at 05:45.** | DSNS, 76916 |
| 7 Oct 21:08 | Same figures as DSNS, with the Desnianskyi district named | Kyiv Operatyvnyi, 198151 |
| 8 Oct 03:54 | Firefighters found the bodies of two people in one damaged apartment; psychologists helped 12 residents | Kyiv Operatyvnyi, 198160 |
| 8 Oct 04:01 | Two killed, citing DSNS | Kyiv24, 153188 |
| 8 Oct 06:19 | Aftermath video; this post reports **five** injured | Kyiv24, 153236 |
| 8 Oct 06:38 | Clean-up under way; two killed | Kyiv24, 153243 |
| 8 Oct 08:02 | Footage of destroyed apartments | Kyiv24, 153262 |
| 8 Oct 08:26 | Part of a wall pushed out by the blast; residents signalled to rescuers from balconies; an operational HQ for residents opened at a nearby school | Kyiv24, 153277 |
| 8 Oct | The HQ location confirmed by two more outlets | Glavcom, life.kyiv.ua |

## 5. Location: district check

Ten posts mention the location, but they do not come from ten independent sources. Kyiv Operatyvnyi's posts repeat the mayor (198147) and the DSNS report (198151). The independent sources that name the district are the **mayor** and **Kyiv24**, which reported from the scene the next morning (posts 153236–153277). Both say Desnianskyi. The DSNS post does not name a district.

The Kyiv Independent ([article](https://kyivindependent.com/russia-hits-another-kyiv-apartment-building-injuring-4/), 7 Oct 22:00 UTC, [archived copy](https://web.archive.org/web/20261020160420/https://kyivindependent.com/russia-hits-another-kyiv-apartment-building-injuring-4/)) wrote that Klitschko reported a drone hit "a 12-story residential building in the city's Darnytskyi district". The mayor's post, published 2.5 hours earlier, says Desnianskyi. Post 7792 was the mayor's last post on 7 October, and his next posts, up to 10:11 UTC on 8 October, are about other strikes; none of them mentions Darnytskyi. Earlier on 7 October the mayor had reported strikes in the Sviatoshynskyi, Solomianskyi and Obolonskyi districts, so several districts were in the news that day. The article's other details (12 storeys, 10th floor, four injured) match the official reports, so the district is most likely a slip in translation or editing. The article still named Darnytskyi when it was archived on 20 October.

The HQ for residents named by three outlets is in the Desnianskyi district, which is consistent with the above. Kyiv24 gave the HQ address with a mistake in the street name; Glavcom and life.kyiv.ua gave the correct one.

## 6. Claims vs. evidence

| Claim (source) | Status | Basis |
|---|---|---|
| Drone strike on a residential building in Kyiv (mayor, DSNS, media) | **Verified** | Consistent official and media reports; footage of the damaged building |
| Desnianskyi district (mayor, Kyiv Operatyvnyi, Kyiv24) | **Verified** | Two independent sources agree; none contradicts |
| Darnytskyi district (Kyiv Independent, attributed to the mayor) | **Likely incorrect** | The mayor's own post says Desnianskyi |
| 4 injured including 2 children; 22 rescued (DSNS) | **Officially reported** | DSNS post (edited version) |
| 2 killed (Kyiv Operatyvnyi; Kyiv24 citing DSNS) | **Reported by two outlets** | The DSNS source post was not collected |
| 5 injured (Kyiv24, 153236) | **Not confirmed** | Single source; DSNS and all other posts say four |

## 7. What was not established

- **The exact building.** The search narrowed to two candidate buildings, but the footage was not used to decide between them: Street View does not cover the courtyards, and the newest street imagery is from 2015. Afterwards, the northern candidate was found to match an independent geolocation published by the GeoConfirmed community. The address is still withheld (section 8).
- **The original DSNS text.** The DSNS post was edited about nine hours after publication. The collection ran 12 days after the event, so only the edited version was preserved; the tool records the edit time but cannot recover earlier versions. Lesson: collect on the day.
- **Where the footage first appeared.** Kyiv Operatyvnyi 198160 and Kyiv24 153188 carry the same 77-second video (checked by viewing both). The files are almost the same size (29.41 MB and 29.42 MB) but their hashes differ, because each channel uploaded its own copy. Kyiv24 credits DSNS, so the footage probably comes from DSNS, but the original post was not found.
- **The DSNS post reporting the deaths.** Kyiv24 cites DSNS for the two deaths, but that post was not collected.
- **Night footage of the fire.** None was found in the channels searched. GeoConfirmed's sources for this event include local Kyiv channels that were not monitored here (kyiv_hey, kievreal1, k_dvizh, kievinfo_kyiv). Lesson: first footage often appears in district-level channels, not in official or large media channels.
- **Satellite data.** Thermal satellite detections (NASA FIRMS) are not suited to a fire in a single apartment building, so they were not used.

## 8. Ethics

- The building address, the candidate building and the HQ address are withheld; only the district is given. People live there, and some were injured or killed.
- Victims are not named. Media files are not published here, only their hashes. Some footage shows destroyed apartments where people died; it was reviewed only as far as the questions required.
- Collection was passive, from a separate research account. No channel or person was contacted.

## Annex A. Collected posts

| Channel | Post | Posted (UTC) | Edited (UTC) | Files | Archived copy |
|---|---|---|---|---|---|
| Vitali Klitschko | [7792](https://t.me/vitaliy_klitschko/7792) | 7 Oct 19:23 | — | 0 | [Wayback](https://web.archive.org/web/20261019171855/https://t.me/vitaliy_klitschko/7792) |
| Kyiv Operatyvnyi | [198147](https://t.me/kyivoperat/198147) | 7 Oct 19:24 | 7 Oct 19:25 | 1 | [Wayback](https://web.archive.org/web/20261019172558/https://t.me/kyivoperat/198147) |
| DSNS | [76916](https://t.me/dsns_telegram/76916) | 7 Oct 21:01 | **8 Oct 05:45** | 8 | [Wayback](https://web.archive.org/web/20261019172219/https://t.me/dsns_telegram/76916) |
| Kyiv Operatyvnyi | [198151](https://t.me/kyivoperat/198151) | 7 Oct 21:08 | 7 Oct 21:08 | 7 | [Wayback](https://web.archive.org/web/20261019172932/https://t.me/kyivoperat/198151) |
| Kyiv Operatyvnyi | [198160](https://t.me/kyivoperat/198160) | 8 Oct 03:54 | 8 Oct 03:54 | 10 | [Wayback](https://web.archive.org/web/20261019173410/https://t.me/kyivoperat/198160) |
| Kyiv24 | [153188](https://t.me/kyivtv/153188) | 8 Oct 04:01 | 8 Oct 04:03 | 4 | [Wayback](https://web.archive.org/web/20261019173818/https://t.me/kyivtv/153188) |
| Kyiv24 | [153236](https://t.me/kyivtv/153236) | 8 Oct 06:19 | 8 Oct 06:19 | 4 | [Wayback](https://web.archive.org/web/20261019174201/https://t.me/kyivtv/153236) |
| Kyiv24 | [153243](https://t.me/kyivtv/153243) | 8 Oct 06:38 | 8 Oct 06:38 | 1 | [Wayback](https://web.archive.org/web/20261019174948/https://t.me/kyivtv/153243) |
| Kyiv24 | [153262](https://t.me/kyivtv/153262) | 8 Oct 08:02 | 8 Oct 08:03 | 5 | [Wayback](https://web.archive.org/web/20261019175333/https://t.me/kyivtv/153262) |
| Kyiv24 | [153277](https://t.me/kyivtv/153277) | 8 Oct 08:26 | 8 Oct 08:27 | 1 | [Wayback](https://web.archive.org/web/20261019180413/https://t.me/kyivtv/153277) |

The media channels edited their posts within three minutes of publishing, which is usual for formatting fixes. The DSNS edit, almost nine hours later, is the only one that may have changed the content.

## Changelog

- v1.0 (21 October 2026): first version.
