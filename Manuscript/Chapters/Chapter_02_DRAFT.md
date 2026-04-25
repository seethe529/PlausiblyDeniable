# Chapter 2 — What I Saw

**Status:** Not Started
**POV:** First person
**Timeline:** Summer 2022 – November 2022

---

## Chapter Goal
Introduce the UAP discovery. Establish what Ryan saw in the data, why it mattered, and what he did about it. Show the transition from routine GIS work to something that couldn't be ignored.

---

## Key Scenes / Beats
- [ ] The moment the data anomaly became undeniable
- [ ] Developing the UAP monitoring prototype
- [ ] The ESRI abstract submission — Matthew Thompson's reaction
- [ ] The growing sense that this work was being noticed
- [ ] Foreshadow the consequences without revealing them yet

---

## Draft

---

# Chapter 2: What I Saw

The tool didn't exist until I made it exist.

That's the thing people don't fully understand about this kind of work. There was no template, no existing system I was adapting or improving. I was writing Python scripts from scratch, in my apartment in Navy Yard, building something that had no predecessor in this specific application. This was before the current wave of AI tools made that kind of development accessible to anyone with a browser and a prompt. It was just me, the language, and a problem that wouldn't leave me alone.

The reports came in through two channels. The first was Skywatch — an internal FAA application I had access to as part of my role. UAP reports filed by pilots and aircraft operators were stored there alongside other sensitive airspace data. The same system housed information regarding President of the United States (POTUS) and Vice President of the United States (VPOTUS) movements — I did not have access to that data, but its presence in the same system speaks to the sensitivity and scope of what Skywatch was. I could filter them by different criteria. Not because anyone told me to. Because the data was there and I was curious and that is what you do when you are a geographer with access to a system that tracks everything moving through national airspace. The second channel was senior leadership, funneling selected reports down through the Air Traffic Control System Command Center. Other analysts were already dashboarding them, and what the dashboards were showing was hard to ignore: UAP reports were increasing at a statistically significant rate. That finding didn't come from me. It came from the institutional apparatus doing what it was built to do — measuring, tracking, flagging. The numbers said something was happening.

My job was to ask what.

The reports that made their way to me came through Matthew Thompson. Aircraft operators, pilots and crew who had seen something they couldn't explain and filed accordingly. By the time they reached me they had already passed through institutional hands. Leadership had looked at them and decided they were worth examining. That pre-selection mattered. These weren't fringe reports scraped from the internet. These were documented encounters that the FAA had determined deserved a closer look.

John Evans was an FAA employee I worked closely with during this period — one of the few people I could show the work to in real time, the only person who saw my excitement as it was happening rather than after the fact. That matters in this kind of work. When you're building something alone, in an apartment, over months, you need at least one person who can look at the screen and understand what they're seeing. John was that person. He was sharp — genuinely technical, the kind of person who could engage with the architecture of what I was building rather than just the surface of it. At one point there was a specific method in the Skyfield library we worked through together — a detail in the implementation that mattered for the geometry to be right. He understood it. That kind of collaboration, small as it was, meant something.

What we were building, eventually, was this: a three dimensional render of the airspace. You could input an aircraft's callsign and altitude — a real flight, a real moment — and the tool would place it in space. Then it would map the orbital paths of satellites against that position. Starlink orbits specifically — the ones whose geometry, at the right sun angle, would produce exactly the kind of anomalous brightness a pilot might report as something unknown.

You could draw a line. Aircraft to satellite. And either the geometry worked — the sun was right, the angle was right, the orbit intersected — or it didn't.

Months of scripting for that. Months of iteration, of running the code and finding what was wrong with it, of slowly building something precise enough to be trusted. At some point Leidos noticed. A short internal broadcast feature landed in my email, a quiet institutional acknowledgment that what I was building was worth knowing about. I bookmarked it. I didn't think too hard about what it meant at the time.

I worked at my standing desk. The apartment was quiet. I had the data and I had the problem and I had time, and I put all three together the way you do when you believe the work is worth doing.

I believed the work was worth doing.

I couldn't stop thinking about it.

That's the honest description of where I was during that period — not stuck, not frustrated, but absorbed in the way you get absorbed when you're building something that keeps revealing itself to you. The work followed me off the clock. Into evenings. Into weekends. I'd step away from the standing desk and the problem would come with me, turning over quietly in the background the way good problems do when you're close to something.

It was on a weekend that it arrived.

My grandmother had a saying she'd used her whole life. Red in the morning, sailors take warning. Red at night, sailors delight. It's an old piece of weather wisdom — the color of the sky at different times of day telling you something about what light is doing, where it's coming from, what it means. She hadn't said it to me recently. She couldn't. She had passed away that summer, while I was deep in this work. But her voice showed up anyway, the way the voices of people we've lost sometimes do — not as memory exactly, but as presence. As something useful arriving from somewhere you didn't expect.

I needed to add sunlight to the orbital paths.

That was what the saying unlocked. The satellite geometry alone wasn't enough. A Starlink satellite passing overhead meant nothing without knowing whether the sun was at the right angle to illuminate it — to turn it from an invisible object in the sky into something bright and anomalous and worth reporting. The light was the variable I hadn't fully accounted for. And once I accounted for it, the tool worked the way I had always believed it could.

Most of the reports resolved. Starlink satellites, sunlit at the right moment, visible from the right altitude and position. Pilots and operators seeing something real — just not something unknown. The tool visualized the orbit segments individually — short discrete lines, each one representing just a few seconds of movement in time, rendered in three dimensional space above the aircraft position. Imagine standing beneath the open sky and seeing those brief segments suspended overhead, each one a snapshot of something moving fast. The geometry explained it. You could see the line between the aircraft and the orbit segment, the sun angle, the moment of intersection. You could see exactly what they had seen and why they had seen it.

My grandmother had spent her whole life reading the sky. She just didn't know she'd one day help someone build a tool that did the same thing.

I wished I could have told her.

On November 1st, 2022, we submitted the abstract.

The full title was "Comparing Reports of Unidentified Aerial Phenomena to Starlink Satellite Orbits." Abstract #1240. Submitted to the 2023 ESRI User Conference, the largest GIS conference in the world, held every year in San Diego. Twenty thousand attendees. The most significant platform in the field.

The names on it were Matthew Thompson, John Evans, and mine. That was Thompson's call. The federal employees had their names on it, and I was the contractor who had built the thing. I didn't argue with the order. I understood how it worked. What mattered was that the work was going out into the world under my name, attached to something real, something that could be evaluated and tested and built upon.

I was beyond excited. This was going to be the biggest moment of my career. The conference was scheduled for July 10th through the 14th in San Diego. I knew there would be preparation: slides, a presentation, the kind of public-facing work that's different from building something alone at a standing desk. I was anxious about that part. But underneath the anxiety was something I hadn't felt in a long time: the certainty that I had done something worth showing.

The tool existed. The work was documented. My name was on it.

A few weeks later, someone forwarded me an email. My screenshots had reached ODNI.

Not every report pointed to a satellite.

That's the part that requires care to describe accurately, because it's easy to overstate and easy to understate, and both would be dishonest. The tool worked on all of them. That's the first thing to understand. It wasn't that the visualization broke down or the methodology failed. It was that when you drew the line — aircraft to orbit segment, sun angle, geometry — sometimes nothing was there. No Starlink constellation at the right position. No sunlit object that could account for what had been reported.

The tool was precise enough to rule satellites out. That's what it was built to do, not just confirm explanations but test them. And some reports didn't confirm.

We weren't the only ones running reports through the tool. I remember at least one other person working through a few themselves — testing the visualization against different sightings, getting familiar with what it could show. When a report came back without a satellite explanation, the response wasn't alarm. It wasn't excitement. It was closer to what any careful researcher feels at the edge of their methodology — a kind of professional acknowledgment that the data had taken us as far as it could.

I remember thinking: there's probably an explanation. We just don't have it yet. That's not a dramatic conclusion. It's an honest one. The absence of a satellite explanation didn't mean the absence of any explanation — it meant we had eliminated one category and whatever remained was outside the scope of what I had built.

We moved on. The work continued. Nobody stopped. Nobody panicked. We noted what the tool had found and what it hadn't, and we kept going.

That's what rigor looks like from the inside. It doesn't feel like revelation. It feels like work.

The tool had one more capability worth describing.

Built into the visualization was a line of sight function — not something I had added as an afterthought, but a deliberate analytical feature. A user could draw their own line. Aircraft to orbit segment. You could take a specific report, place the aircraft in three dimensional space at its logged altitude and callsign, and then manually trace the geometry yourself — pulling a line from the cockpit position out toward the orbit segments suspended above it, testing whether the angle worked, whether the light worked, whether what the pilot had seen could be accounted for by what was moving overhead.

It was designed to give the analyst agency. Not just to run reports through an automated filter but to interrogate individual cases by hand, to bring human judgment into contact with the data at the level of a single sighting. You could see what the pilot would have seen. You could test it yourself.

I had sent screenshots of the visualization to people within the FAA. That was normal. The work was being shared, discussed, passed around in the way that work gets passed around when people find it useful. I didn't think too hard about where the screenshots were going. I was focused on the tool.

A few weeks before March 2nd, Gary Miller, Director of Air Traffic Organization (ATO) Security, AJR2, made me aware that my screenshots had reached ODNI. The Office of the Director of National Intelligence is not a place that receives routine contractor work. It sits above the CIA, the NSA, the DIA, and fourteen other federal intelligence agencies - the apex of the entire apparatus. For a Python script built at a standing desk in a Navy Yard apartment to land there meant someone, somewhere above my clearance level, had decided it was worth passing up.

I don't know who sent them. I don't know what was said about them. What I know is that the email made its way to me, and I saw his name on it.

I went back to my standing desk after that. The apartment was quiet. The tool was running. Outside, the city moved the way it always did, oblivious, unhurried, unconcerned with what was happening in a Navy Yard apartment twenty minutes from the White House.

Two weeks later they made me transfer the code.

---

## Notes / Research Needed
- Cross-reference: `IPASS_AbstractAcceptedESRI_2023.pdf`
- Cross-reference: `HPSCI_Fitzpatrick_20240307_0930.pdf`
- Cross-reference: `Lingo_Master_Evidence_Timeline_v4.pdf` — Summer/Fall 2022 entries
