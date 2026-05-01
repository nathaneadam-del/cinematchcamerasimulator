# Magic Hour: Camera Simulator — Image Generation Guide

Each image is permanently assigned a specific camera archetype. Generate each image so its
visual content matches the archetype's lighting, depth of field, focal length, and motion context.
Students will look at the image and figure out the correct settings — so the visual cues must be
consistent with the archetype listed below each prompt.

---

## ARCHETYPE REFERENCE TABLE

| # | FPS | Shutter | Lens | Aperture | WB | EV | Notes |
|---|-----|---------|------|----------|----|----|-------|
| 0 | 24  | 1/50    | 85mm | f/2.8 shallow | 5600K daylight | 15 | Needs ND6 filter |
| 1 | 24  | 1/50    | 50mm | f/1.4–2.8 shallow | 3200K tungsten | 12 | Warm interior |
| 2 | 24  | 1/50    | 24mm | f/8+ deep | 3200K tungsten | 10 | Wide interior |
| 3 | 24  | 1/50    | 24mm | f/8+ deep | 4500K overcast | 8  | Overcast exterior |
| 4 | 24  | 1/50    | 50mm | f/1.4–2 shallow | 3200K tungsten | 6  | Night/dim intimate |
| 5 | 60  | 1/120   | 85mm | f/2.8 shallow | 5600K daylight | 16 | Slow-mo, needs ND6 |
| 6 | 60  | 1/120   | 24mm | f/8+ deep | 5600K daylight | 13 | Slow-mo wide action |
| 7 | 60  | 1/120   | 35mm | f/1.4–2.8 shallow | 4500K overcast | 11 | Slow-mo overcast |
| 8 | 60  | 1/120   | 85mm | f/1.4–2 shallow | 3200K tungsten | 9  | Slow-mo dim interior |
| 9 | 60  | 1/120   | 24mm | f/8+ deep | 4500K overcast | 7  | Slow-mo dusk wide |
|10 | 120 | 1/250   | 50mm | f/2–2.8 shallow | 5600K daylight | 16 | Extreme slow-mo bright |
|11 | 120 | 1/250   | 14mm | f/8+ deep | 5600K daylight | 14 | Extreme slow-mo ultra-wide |
|12 | 120 | 1/250   | 85mm | f/2.8 shallow | 4500K overcast | 13 | Extreme slow-mo overcast |
|13 | 120 | 1/250   | 35mm | f/8+ deep | 3200K tungsten | 10 | Extreme slow-mo interior |
|14 | 120 | 1/250   | 85mm | f/1.4–2 shallow | 4500K overcast | 8  | Extreme slow-mo dusk |

---

## GENERATION TIPS

**Visual cues to embed in each image:**
- **5600K (daylight):** Clean, neutral, bright outdoor sun — no colour cast
- **4500K (overcast):** Flat grey sky, soft diffused shadows, cool neutral tones
- **3200K (tungsten):** Warm orange/amber interior light from lamps or practicals
- **Shallow DoF:** Background clearly blurred, subject sharply isolated
- **Deep DoF:** Everything sharp from foreground to background
- **Slow-mo context:** Subject mid-motion (athlete, dancer, object in air) even if frozen
- **High-speed context:** Motion detail that suggests ultra-high-frame-rate capture

**Format:** Use `--ar 16:9` in Midjourney. Aim for photographic/cinematic realism.
Name files `image-01.jpeg` through `image-50.jpeg` to match `images.json`.

---

## IMAGE 01 — Archetype 0 (24fps | 85mm | 5600K daylight | shallow DoF | EV 15)

A woman in her late 20s photographed outdoors on a bright sunny afternoon. Shot on 85mm equivalent, creating natural background compression. She is in sharp focus; the sunlit garden or park behind her is completely blurred into smooth golden bokeh. Direct overhead sunlight creates clean, bright skin tones. The image is noticeably bright — the kind of shot where an ND filter would be essential. Pure daylight colour temperature, no warm cast.

---

## IMAGE 02 — Archetype 5 (60fps | 85mm | 5600K daylight | shallow DoF | EV 16)

A dancer or gymnast captured mid-movement outdoors in blazing afternoon sun. Shot at 85mm with shallow depth of field — the performer is sharp, the blurred background of bright sky and foliage shows heavy bokeh. The scene is extremely bright, suggesting slow-motion capture potential. Pure daylight, strong directional sunlight. Background is completely thrown out of focus.

---

## IMAGE 03 — Archetype 10 (120fps | 50mm | 5600K daylight | shallow DoF | EV 16)

A splash of water thrown into the air in direct bright sunlight, photographed at a standard 50mm perspective. Crystal-clear water droplets are frozen in mid-air, with the blurred bright background behind them. Very high ambient light — blazing sun overhead. The moment feels frozen, suggesting extreme high-speed capture. Shallow depth of field isolates the splash. Daylight colour temperature.

---

## IMAGE 04 — Archetype 1 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 12)

A person reading a novel in an armchair, lit entirely by a warm table lamp beside them. The room has a distinctly warm amber/orange colour cast from the tungsten bulb. Shot at a standard 50mm perspective, shallow depth of field with the reader sharp and the bookshelf behind them softly blurred. The warm interior glow is prominent — no daylight. Well-lit for an interior.

---

## IMAGE 05 — Archetype 6 (60fps | 24mm | 5600K daylight | deep DoF | EV 13)

Beach volleyball players leaping for the ball in bright afternoon sunlight. Shot wide at 24mm, capturing the players, the net, the sand, and the bright blue sky — all in sharp focus from foreground to background. Strong direct daylight, clean colour temperature. The dynamic action suggests slow-motion potential. No blur in the background — deep field throughout the frame.

---

## IMAGE 06 — Archetype 11 (120fps | 14mm | 5600K daylight | deep DoF | EV 14)

Ocean waves crashing on a beach photographed with an ultra-wide 14mm lens. The foreground foam, mid-ground breaking wave, and distant horizon are all equally sharp. Bright direct sunlight, clean daylight colour. The wide perspective creates visible barrel distortion. The scale and energy suggests high-speed capture potential. Deep focus throughout — nothing soft or blurred.

---

## IMAGE 07 — Archetype 2 (24fps | 24mm | 3200K tungsten | deep DoF | EV 10)

A large, warmly lit living room photographed with a wide 24mm lens. Every element is in sharp focus — from the sofa in the foreground to the bookshelf and windows on the far wall. Warm tungsten practicals (lamps, overhead fixtures) cast an amber glow throughout. Deep depth of field, everything equally readable. No blurred elements. Interior-lit, no daylight.

---

## IMAGE 08 — Archetype 7 (60fps | 35mm | 4500K overcast | shallow DoF | EV 11)

A street performer or acrobat captured mid-gesture on a cloudy day. Shot at 35mm, showing the subject at medium range with a softly blurred background of buildings or crowd. Flat, diffused overcast light — no hard shadows, slightly cool neutral tones from cloud cover. The scene suggests slow-motion potential. Background gently out of focus, subject sharp.

---

## IMAGE 09 — Archetype 12 (120fps | 85mm | 4500K overcast | shallow DoF | EV 13)

A sprinter or boxer captured mid-action under flat overcast grey sky. Shot at 85mm with shallow depth of field — the athlete is sharp, the background (track or gym exterior) is blurred. Soft, directionless overcast light, cool neutral colour temperature. The frozen motion detail suggests extreme high-speed capture. No harsh shadows. Shallow bokeh in the background.

---

## IMAGE 10 — Archetype 3 (24fps | 24mm | 4500K overcast | deep DoF | EV 8)

An urban street scene on a flat grey overcast day. Buildings, parked cars, pedestrians, and street signs are all visible and in sharp focus throughout the frame. Wide 24mm perspective. Muted, neutral colours from cloud cover — no harsh shadows, no warm cast. Everything equally sharp from the foreground pavement to the distant buildings. Slightly dim due to heavy cloud cover.

---

## IMAGE 11 — Archetype 8 (60fps | 85mm | 3200K tungsten | shallow DoF | EV 9)

A bartender shaking a cocktail in a dimly lit bar. Shot at 85mm, the bartender's motion is sharp, the warm bokeh of bar shelves and bottles blurs into the background. Warm amber tungsten light from practicals — clearly interior. The image is somewhat dim. Background lights create soft warm bokeh. Slow-motion potential in the hand movement. Intimate, moody atmosphere.

---

## IMAGE 12 — Archetype 13 (120fps | 35mm | 3200K tungsten | deep DoF | EV 10)

Factory machinery or industrial equipment in operation, photographed in a warm-lit warehouse. Shot at 35mm with deep focus — both the foreground equipment and the background machinery are sharp. Warm amber tungsten overhead lighting. The mechanical motion suggests high-speed capture. Everything in focus. Interior tungsten colour cast throughout.

---

## IMAGE 13 — Archetype 4 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 6)

A person sitting alone by a single warm candle or table lamp at night. The room is nearly dark — the warm light source illuminates just the subject's face and hands. Shot at 50mm with very shallow depth of field. The background falls away into darkness. Deep warm amber colour cast. Intimate, quiet mood. The image is quite dark overall — only the subject and immediate surroundings visible.

---

## IMAGE 14 — Archetype 9 (60fps | 24mm | 4500K overcast | deep DoF | EV 7)

A city street at twilight, photographed wide at 24mm. Street lights and shop windows are just turning on. The sky is transitioning from blue hour to dusk — cool overcast tones. Everything is in sharp focus: the foreground pavement, people walking, illuminated shopfronts, and the distant skyline. The overall scene is dim — the ambient light is low. Deep field, everything readable.

---

## IMAGE 15 — Archetype 14 (120fps | 85mm | 4500K overcast | shallow DoF | EV 8)

A sparkler or handheld light source being waved at dusk. Shot at 85mm with shallow depth of field — the glowing sparkler is sharp, the dusk cityscape behind it is blurred into soft bokeh. Blue hour sky with cool grey-blue tones. The frozen motion of the light trail suggests extreme slow-motion capture. Overcast/dusk colour temperature. Background city lights create soft circular bokeh.

---

## IMAGE 16 — Archetype 0 (24fps | 85mm | 5600K daylight | shallow DoF | EV 15)

A male photographer or creative professional photographed outdoors in strong midday sunlight. 85mm equivalent perspective, head and shoulders framing. Very shallow depth of field — subject sharp, urban background completely blurred and creamy. Clean, bright daylight colour temperature. No warm cast. The extreme brightness suggests this scene requires an ND filter.

---

## IMAGE 17 — Archetype 5 (60fps | 85mm | 5600K daylight | shallow DoF | EV 16)

A track athlete crossing a finish line in blazing afternoon sunlight. Shot at 85mm, the runner in sharp focus, the crowd and stadium in the blurred background. Extremely bright direct sunlight — shadows are hard and short. The frozen motion of the runner's expression and posture suggests slow-motion capture. Very bright exposure — daylight at full intensity.

---

## IMAGE 18 — Archetype 10 (120fps | 50mm | 5600K daylight | shallow DoF | EV 16)

Coloured confetti or paint powder erupting into bright afternoon air. Shot at 50mm with shallow depth of field — the confetti cloud is sharp, the bright outdoor background is blurred. Extremely bright direct sunlight. The frozen detail of each confetti piece suggests extreme high-speed capture. Very high ambient light, clean daylight colour temperature.

---

## IMAGE 19 — Archetype 1 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 12)

A person writing in a notebook or journal at a wooden desk illuminated by a warm desk lamp. Interior scene with a prominent orange/amber colour cast from the tungsten light source. Shot at 50mm, shallow depth of field keeps the writer sharp and blurs the warm-lit room behind. Well-lit for a tungsten interior. No daylight — purely warm practical lighting.

---

## IMAGE 20 — Archetype 6 (60fps | 24mm | 5600K daylight | deep DoF | EV 13)

Children playing in a park fountain on a bright sunny day. Wide 24mm perspective showing the full scene — kids, fountain, trees, and sky all in sharp focus. Strong direct daylight, clean colour temperature, hard shadows. The dynamic splashing and running suggests slow-motion potential. No blurred elements — everything sharp from front to back.

---

## IMAGE 21 — Archetype 11 (120fps | 14mm | 5600K daylight | deep DoF | EV 14)

A crowd at an outdoor festival or concert in bright midday sun, photographed with a 14mm ultra-wide lens. The foreground crowd, mid-ground stage, and background sky are all equally sharp. Visible ultra-wide distortion. Strong direct sunlight, clean daylight. The energy of the crowd suggests high-speed capture potential. Deep field throughout — nothing blurred.

---

## IMAGE 22 — Archetype 2 (24fps | 24mm | 3200K tungsten | deep DoF | EV 10)

A home workshop or studio photographed with a wide 24mm lens. Workbenches, shelves of tools or art supplies, and the far wall are all in sharp focus. Warm tungsten overhead fixtures provide the only light — amber colour cast throughout. Deep depth of field, everything equally readable from front to back. No daylight. Interior domestic space.

---

## IMAGE 23 — Archetype 7 (60fps | 35mm | 4500K overcast | shallow DoF | EV 11)

A cyclist in motion on a quiet road under a heavy grey sky. Shot at 35mm, the cyclist is sharp, the blurred road and hedgerows behind suggest moderate shallow depth of field. Flat, diffused overcast light — no shadows, cool neutral tones. Slow-motion potential in the spinning wheels and flowing clothing. Background softly out of focus.

---

## IMAGE 24 — Archetype 12 (120fps | 85mm | 4500K overcast | shallow DoF | EV 13)

A tennis player mid-serve on an outdoor court under flat overcast sky. Shot at 85mm, the player sharp, the background court and crowd blurred. Soft, directionless grey light — cool neutral overcast colour. The extreme detail in the motion (ball, racket, hair) suggests 120fps capture. No harsh shadows. Shallow background bokeh.

---

## IMAGE 25 — Archetype 3 (24fps | 24mm | 4500K overcast | deep DoF | EV 8)

An outdoor market on a dull cloudy day. Stalls, vendors, and shoppers are all in sharp focus throughout the wide 24mm frame. Flat, soft overcast light — muted colours, no shadows. The sky is visibly grey and overcast. The scene is somewhat dim from heavy cloud cover. Deep field — foreground stalls and distant buildings equally sharp.

---

## IMAGE 26 — Archetype 8 (60fps | 85mm | 3200K tungsten | shallow DoF | EV 9)

A person playing piano in a dimly lit room, lit only by a warm lamp beside the piano. Shot at 85mm, the player's hands in motion are sharp, the warm bokeh of the room dissolves behind. Intimate warm amber light — clearly tungsten practical. The scene is quite dim. Background lamp light creates soft circular bokeh. Slow-motion potential in the hand movement.

---

## IMAGE 27 — Archetype 13 (120fps | 35mm | 3200K tungsten | deep DoF | EV 10)

A glass or ceramic object shattering in a warmly lit studio, photographed at 35mm. The broken pieces in the foreground and the studio background are both in focus. Warm tungsten studio lighting creates an amber glow throughout. The detail of the shattering object suggests high-speed capture. Everything sharp. Interior colour cast.

---

## IMAGE 28 — Archetype 4 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 6)

Two people at a candlelit restaurant table, late at night. The scene is very dark — only the candle flame and its warm amber glow illuminate the subjects. Shot at 50mm, shallow depth of field, the faces softly lit and in focus, the dark restaurant background melting away. Deeply warm colour cast. Very low ambient light. Romantic, intimate atmosphere.

---

## IMAGE 29 — Archetype 9 (60fps | 24mm | 4500K overcast | deep DoF | EV 7)

A riverside promenade at twilight, photographed wide at 24mm. Streetlights are on, the sky is deep blue, reflected in the water. Buildings, walkway, and distant bridge all in sharp focus. The overall scene is dim — blue hour transitional light. Cool overcast/blue hour colour temperature. Deep field, everything equally visible.

---

## IMAGE 30 — Archetype 14 (120fps | 85mm | 4500K overcast | shallow DoF | EV 8)

A musician playing guitar outdoors at dusk. Shot at 85mm — the musician and guitar are sharp, the blue hour sky and distant city blur behind. Cool atmospheric dusk light, overcast colour temperature. The frozen detail of the strumming hand suggests extreme slow-motion capture. Background city lights begin to form soft bokeh. Moody twilight atmosphere.

---

## IMAGE 31 — Archetype 0 (24fps | 85mm | 5600K daylight | shallow DoF | EV 15)

Two hikers on a mountain trail pausing to look at the view, photographed at 85mm. Very shallow depth of field — the subjects are sharp, the sunlit mountain landscape behind them is completely blurred into creamy bokeh. Strong direct sunlight, clean daylight colour temperature. The extreme brightness of the background bokeh emphasises how much light there is — an ND filter scene.

---

## IMAGE 32 — Archetype 5 (60fps | 85mm | 5600K daylight | shallow DoF | EV 16)

A person leaping or jumping in a sunny park, captured mid-air at 85mm. Very shallow depth of field — the airborne subject is sharp, the bright sunlit background completely blurred. Blazing afternoon sun, clean daylight. The frozen expression and posture suggests slow-motion. Very high ambient light level. Background summer foliage forms golden bokeh.

---

## IMAGE 33 — Archetype 10 (120fps | 50mm | 5600K daylight | shallow DoF | EV 16)

A dog shaking water off its fur in bright sunlight, photographed at 50mm. The dog is sharp, the flying water droplets are frozen in crystal clarity, and the bright outdoor background is blurred. Very high ambient light — direct sun. The extraordinary detail in the water droplets suggests extreme high-speed capture. Background completely out of focus.

---

## IMAGE 34 — Archetype 1 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 12)

A craftsperson painting or sculpting in a studio lit by warm tungsten overhead lights and work lamps. Shot at 50mm with shallow depth of field — the artist and their work are sharp, the warm studio background softly blurred. Strong amber/orange colour cast from the tungsten sources. Well-lit interior. No daylight — purely warm practical and studio lighting.

---

## IMAGE 35 — Archetype 6 (60fps | 24mm | 5600K daylight | deep DoF | EV 13)

Skateboarders at an outdoor skate park on a bright sunny day. Wide 24mm perspective showing multiple riders, ramps, and the sky — all in sharp focus. Hard directional sunlight, clean daylight colour. The dynamic mid-trick poses suggest slow-motion potential. No blurred background — everything from foreground rail to distant trees equally sharp.

---

## IMAGE 36 — Archetype 11 (120fps | 14mm | 5600K daylight | deep DoF | EV 14)

A busy city intersection photographed with a 14mm ultra-wide lens in bright midday sun. Foreground pavement, mid-ground traffic and pedestrians, background skyscrapers all in equal sharp focus. Strong direct sunlight, visible ultra-wide lens distortion. The frozen moment of urban activity suggests high-speed capture. Nothing blurred — deep field throughout.

---

## IMAGE 37 — Archetype 2 (24fps | 24mm | 3200K tungsten | deep DoF | EV 10)

A large restaurant dining room photographed with a 24mm wide-angle lens. Tables, chairs, artwork on the walls, and the distant bar are all in sharp focus throughout. Warm tungsten overhead fixtures bathe everything in amber light. Deep field — foreground and background equally sharp. Interior only, no daylight. Well-lit for an indoor environment.

---

## IMAGE 38 — Archetype 7 (60fps | 35mm | 4500K overcast | shallow DoF | EV 11)

A person running through a city street in rain, photographed at 35mm on an overcast day. The runner is sharp, the grey wet buildings behind them slightly blurred. Flat diffused overcast light, rain creating texture. Cool neutral colour temperature. The motion of the runner and rain droplets suggests slow-motion potential. Soft background separation.

---

## IMAGE 39 — Archetype 12 (120fps | 85mm | 4500K overcast | shallow DoF | EV 13)

A martial artist or dancer captured mid-kick or mid-leap outdoors under a grey overcast sky. Shot at 85mm — the person is perfectly sharp, the background training ground or urban space blurs behind. Soft diffused overcast light, cool neutral tones, no shadows. Every detail of the extreme motion is frozen — suggests 120fps capture. Shallow background bokeh.

---

## IMAGE 40 — Archetype 3 (24fps | 24mm | 4500K overcast | deep DoF | EV 8)

A public plaza or town square on a heavily overcast day. Wide 24mm perspective showing benches, sculptures, buildings, and the grey sky — all in sharp focus. Flat, muted colours from the thick cloud cover. The scene is noticeably dim. Deep field throughout, everything equally visible from foreground cobblestones to distant architecture. Cool neutral colour temperature.

---

## IMAGE 41 — Archetype 8 (60fps | 85mm | 3200K tungsten | shallow DoF | EV 9)

A chef plating food in a restaurant kitchen lit by warm overhead practicals. Shot at 85mm, the chef's hands in motion are sharp, the warm bokeh of the kitchen background dissolves behind. Distinctly amber/warm colour cast from tungsten kitchen lighting. The scene is dim but intimate. Slow-motion potential in the hand movements. Background out of focus.

---

## IMAGE 42 — Archetype 13 (120fps | 35mm | 3200K tungsten | deep DoF | EV 10)

Steam or smoke rising from a pot or machine in a warmly lit workshop, photographed at 35mm. The steam patterns and the room behind it are both in focus — deep field. Warm amber tungsten workshop lighting. The fluid motion of the steam suggests high-speed capture would reveal extraordinary detail. Interior colour cast. Everything sharp front to back.

---

## IMAGE 43 — Archetype 4 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 6)

A person reading at a desk in a nearly dark room, lit only by a small warm desk lamp. Shot at 50mm — the person's face and the open book are sharp, everything beyond them dissolves into darkness. Very warm amber light from the single tungsten source. Very low overall brightness. Intimate, quiet mood. The dark surroundings make the subject feel isolated and focused.

---

## IMAGE 44 — Archetype 9 (60fps | 24mm | 4500K overcast | deep DoF | EV 7)

An outdoor street food market at dusk. Wide 24mm shot showing stalls, vendors, and customers with warm artificial stall lighting mixing with the cool blue evening sky. The whole scene is in sharp focus — stalls in the foreground, buildings and sky in the background. Transitional light — blue dusk overhead, warm tungsten at stall level. The scene is quite dim overall.

---

## IMAGE 45 — Archetype 14 (120fps | 85mm | 4500K overcast | shallow DoF | EV 8)

A figure skater or dancer on an outdoor stage at dusk, photographed at 85mm. The performer is sharply frozen mid-spin, the blue hour sky and distant audience blurring behind. Cool overcast/twilight colour temperature. Every detail of the spinning costume is frozen — suggests extreme slow-motion capture. Background becomes soft bokeh. Atmospheric dusk mood.

---

## IMAGE 46 — Archetype 0 (24fps | 85mm | 5600K daylight | shallow DoF | EV 15)

A chef being photographed outside their restaurant on a bright afternoon. 85mm portrait framing, shoulders up. The subject is tack sharp, the sunlit street behind completely blurred into creamy bokeh. Strong direct midday sun, clean daylight colour temperature. The extreme brightness of the shot is evident — an ND filter would be essential here.

---

## IMAGE 47 — Archetype 1 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 12)

Two friends having a conversation in a warmly lit kitchen at night. Shot at 50mm, medium framing showing both people in mild shallow focus — the nearer person sharp, the one behind slightly softer. Warm amber light from overhead fixtures. Distinctly indoor tungsten colour cast. Well-lit for an interior. Background kitchen elements softly out of focus.

---

## IMAGE 48 — Archetype 2 (24fps | 24mm | 3200K tungsten | deep DoF | EV 10)

A hotel corridor or apartment hallway photographed with a 24mm wide-angle lens. The patterned carpet in the foreground, doors along the side walls, and the far end of the corridor are all in sharp focus. Warm tungsten overhead lighting creates an amber glow. Deep field throughout. Nothing blurred. Interior, no daylight.

---

## IMAGE 49 — Archetype 3 (24fps | 24mm | 4500K overcast | deep DoF | EV 8)

A residential street on a grey overcast morning. Houses, parked cars, trees, and the cloudy sky visible in a wide 24mm shot — all elements in sharp focus. Flat, muted colour palette from the cloud cover. Slightly underlit from the heavy overcast. No shadows. Deep field from the foreground path to the distant end of the street. Cool neutral colour temperature.

---

## IMAGE 50 — Archetype 4 (24fps | 50mm | 3200K tungsten | shallow DoF | EV 6)

A person sitting at a bar counter late at night, lit by a single warm overhead light. Shot at 50mm, the subject is in focus, the dark bar receding behind into warm bokeh from distant bottles and glasses catching light. Very warm amber colour cast. Low ambient light — the bar is dim. Only the immediate surroundings are visible; everything else dissolves into shadow.

---

## ARCHETYPE-TO-IMAGE MAPPING (quick reference)

| Archetype | Images |
|-----------|--------|
| 0 — Bright 85mm portrait, 24fps, 5600K, shallow | 01, 16, 31, 46 |
| 1 — Warm interior 50mm, 24fps, 3200K, shallow | 04, 19, 34, 47 |
| 2 — Wide interior 24mm, 24fps, 3200K, deep | 07, 22, 37, 48 |
| 3 — Overcast street 24mm, 24fps, 4500K, deep | 10, 25, 40, 49 |
| 4 — Night intimate 50mm, 24fps, 3200K, shallow | 13, 28, 43, 50 |
| 5 — Slow-mo bright portrait 85mm, 60fps, 5600K, shallow | 02, 17, 32 |
| 6 — Slow-mo wide action 24mm, 60fps, 5600K, deep | 05, 20, 35 |
| 7 — Slow-mo overcast 35mm, 60fps, 4500K, shallow | 08, 23, 38 |
| 8 — Slow-mo dim interior 85mm, 60fps, 3200K, shallow | 11, 26, 41 |
| 9 — Slow-mo dusk wide 24mm, 60fps, 4500K, deep | 14, 29, 44 |
| 10 — Extreme slow-mo bright 50mm, 120fps, 5600K, shallow | 03, 18, 33 |
| 11 — Extreme slow-mo ultra-wide 14mm, 120fps, 5600K, deep | 06, 21, 36 |
| 12 — Extreme slow-mo overcast 85mm, 120fps, 4500K, shallow | 09, 24, 39 |
| 13 — Extreme slow-mo interior 35mm, 120fps, 3200K, deep | 12, 27, 42 |
| 14 — Extreme slow-mo dusk 85mm, 120fps, 4500K, shallow | 15, 30, 45 |
