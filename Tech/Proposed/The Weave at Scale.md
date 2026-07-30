---
title: The Weave at Scale
version: "1.0"
status: "proposal — direction, not commitment"
date: 2026-07-29
part_of: ARC V1 Corpus
author: Daniel Thorson
---

# The Weave at Scale

*A proposal for how the Weekly Weave might develop across the earned doublings. The [[ARC Weekly Weave — Design Specification|Weekly Weave]] is the ARC's only live system; everything here is horizon, not plan.*

The Weave that is live today was built for a network of dozens growing toward 150: one weekly cycle, one pool, one steward's Saturday review, one release. Its own specification ends with a section called *Known limits and open work*, and that section is the honest ground of this document. The answers to scale should grow from observed use, member experience, and steward learning. What follows is not a roadmap. It is the shape of the questions we expect to meet, held loosely enough that reality can correct them.

The network grows one earned doubling at a time, and only when the field can carry it. The Weave grows the same way.

## What does not change

Five invariants hold at every scale. A version of the Weave that cannot honor them is not a bigger Weave; it is a different and worse system wearing its name.

**The human release threshold.** No cycle goes out unless a person inside the practice has reviewed and approved it. At larger scale this threshold multiplies, into more stewards and more reviews, but it never automates away. The system prepares; a human releases.

**Private boundaries.** A member can say *not this person* without justifying it to the system, to a steward beyond the recording of it, or to the other person. Boundaries persist, are never visible to anyone they concern, and outrank every optimization at every size.

**No reputation system.** No scores, no reliability ratings, no desirability ranking, no participation counts, nothing that lets the system or anyone reading it decide who is a good member. Check-ins remain private, remain unrated, and never become matching inputs.

**Legibility.** The matcher stays deterministic and explainable. Any pairing can be accounted for after the fact in plain language. If a proposed improvement makes the weave better and inexplicable, the answer is no.

**Designed to be left.** Members spend almost no time in the system and all their time in encounter. Growth pressure runs the other way, toward apps, feeds, presence, and engagement, and is refused at every threshold.

## Formed practitioners in the weave

The first real change we can see coming is not about volume. It is about formation.

As Practice Holders emerge, the weave gains a new care: newer members should regularly find themselves practicing with formed practitioners, including Practice Holders, rather than meeting only other newcomers. Not as instruction, and never announced as such — the introduction email would not say who is formed and who is new — but as the quiet hospitality of a field that receives its arrivals well.

Concretely this is one added weight in the matcher, tunable by stewards and visible to them: alongside the preference for novelty, a preference for pairing a newer member with a formed practitioner when they have not encountered one recently. The weight bends the weave; it does not create tiers of member, and no member ever sees it.

## Repeats, byes, and the texture of a larger pool

At today's size, the matcher manages scarcity. Repeats are sometimes unavoidable, byes fall unevenly when availability is tight, and the priorities exist to distribute that scarcity fairly.

At 600 or 1,200, the problem inverts. Novelty becomes abundant, since no one could meet everyone, and the matcher's work becomes the texture of each member's encounters over time: enough new people that the network keeps meeting itself, enough spacing that repeats feel like return rather than rut, byes rare and fairly rotated. The live spec already names repeat spacing and bye distribution as things to review through real use; whatever we learn at 150 becomes the ground for how they are held at 300.

## The member's experience does not scale

Whatever changes underneath, the member's experience should be indistinguishable at 1,200 from what it is at 50: an email arrives with a name and the times you share, you reply all, you meet, and on Friday a private question asks how it went. No accounts appear, no app appears, no profile grows richer, no feed forms around the practice.

This is a constraint on the engineering, not a hope. Every scaling pressure has an easy answer that adds a surface — a dashboard for members, a directory, a presence indicator — and each of those answers is refused in advance. The system may become more capable. The member's encounter with it stays this small.

The same holds for what a matched pair can see of each other: a name, an email address, the windows they share. Full schedules, flexibility, notes, boundaries, and history stay private at every size, and the check-in stays a private conversation between a member and the stewards.

## Held loosely: 300, 600, 1,200

**Around 300**, geography becomes real. Members span enough time zones that a single pool starts producing pairs with almost no shared waking hours, and the strict overlap rule starts generating byes it should not. The likely questions: whether the weave should band by time zone, whether availability needs richer expression, and whether one steward's Saturday morning is still enough. Perhaps this is where a second steward joins the rhythm.

**Around 600**, the single weekly cycle itself comes into question. Regional weaves, each with its own steward and its own release, woven occasionally into cross-regional cycles so the regions do not become islands? A stewarding body rather than a steward, with its own practice of review? We do not know, and we are suspicious of anyone who claims to from here.

**Around 1,200**, the Weave is infrastructure a network genuinely depends on, and the questions become institutional: how stewards are formed and relieved, how the field-health view is shared without becoming surveillance, whether the Gathering itself has become plural and what that does to the rhythm the Weave is anchored to. These are questions for the people who will be there, informed by everything learned on the way.

None of these thresholds is a commitment. Each doubling is earned, and each pause is a real possibility. The Weave at 150 serving depth is worth more than the Weave at 1,200 serving throughput.

## Stewards multiply before systems do

One conviction runs through every threshold: when the Weave strains, the first response is human, not technical. A pool too large for one steward's Saturday morning is met by a second steward before it is met by an approval algorithm. A region whose rhythm no longer fits the anchor cycle is met by a person who knows that region, not by a timezone setting.

Stewarding is itself a formation. Whoever tends the weave holds a quiet power over who encounters whom, and the discipline that governs it now — that stewards are inside the practice, that their selections are invisible to members, that boundaries are honored without question — is what a future body of stewards would be formed in. How that formation works is unknown from here, and it is one of the more consequential unknowns on this page.

## How stewards feel the weave

At every scale, the people tending the Weave need to feel whether it is serving. Today that feeling comes from a small pool a steward can hold in mind. At larger scale it needs help: a field-health view that shows, in aggregate, whether pairs are meeting, how byes are falling, whether newer members are encountering formed practitioners, where availability is thinning the weave.

The line that must hold: this view describes the weave, never the members. Aggregate rates, coverage, distribution — yes. Per-person scores, individual reliability, anyone's history dressed as a metric — never. It is a window for tending, not a scoreboard, and members are told plainly that it exists and what it can and cannot see.

## Where the answers come from

Every question above has the same source of truth: the network practicing at its current size. The live spec's open work is the near ground of this whole horizon: a settled deletion schedule for every class of Weave data, an independent support channel distinct from ordinary stewardship, richer handling of one-off travel and exceptions, and a real review of how the matching priorities behave in use — repeat spacing, bye distribution, whether the availability model is enough. Those come before any of the doublings do, and what they teach will reshape what the doublings ask.

The live specification's closing discipline governs here too: any change should answer a demonstrated member or steward need while preserving the service's legibility and restraint. Scale is not a design problem to be solved in advance. It is a series of thresholds at which the network, knowing more than we know now, decides again what the Weave should be.

This proposal draws its real ideas from two archived prototypes, *ARC Routing System — Scale Extrapolation* and *ARC Routing System v1 — Design & Build Plan*, which remain in Archive/Pre-V1 (2026-07)/Tech as lineage.
