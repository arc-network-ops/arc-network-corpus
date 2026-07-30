---
title: "ARC Weekly Weave — Design Specification"
tags:
- arc-network
- weekly-weave
- coordination-layer
created: 2026-07-29
status: live — corpus specification
version: "1.0"
author: Daniel Thorson (source and product direction); completed against the live build by Codex
audience: members, prospective members, collaborators; V1 Corpus companion
live_url: https://www.arcnetwork.is/weave
---

# ARC Weekly Weave — Design Specification

> The live system routing members into regular dyadic practice. — *Network Spec v1, companion list*

## 1. What it is

The Weekly Weave is the coordination layer's first live expression. Each week it matches ARC members into pairs for dyadic unfolding and introduces them by email. They take it from there.

It is warm infrastructure for encounter. Its purpose is to let the practice happen with as little friction as possible: to move people into relationship and then get out of the way. It is not a social space, a destination, or an app to check. Members do not create passwords or maintain accounts. The Weave succeeds when members spend almost no time in the system and their time in encounter with each other.

The V1 service is live at [arcnetwork.is/weave](https://www.arcnetwork.is/weave). The weekly clock is automated, but every set of pairings is reviewed and released by a human steward.

## 2. The member experience

### Joining

A member joins through the Weekly Weave enrollment page or, when needed, a private invitation from a steward. Joining the Weave creates a routing profile; it does not itself confer ARC membership.

The member gives:

- their name, email address, and time zone;
- the recurring windows in which a one-hour practice could begin;
- how flexible they are beyond those windows;
- an optional private scheduling note for the stewards;
- their agreement to the Weekly Weave data policy and participation terms.

Once active, the member remains in the weekly rotation until they pause or leave. There is no weekly acceptance step.

### Receiving a weave

On Saturday afternoon, each matched pair receives one shared introduction email. It names both people, shows the recurring times they have in common, and asks them to reply all to choose a time, link, and place for the encounter.

The shared times appear in each person's own time zone. The system never reveals either person's full schedule, flexibility setting, or private note.

If the system cannot make an eligible match, the member receives a simple bye email. A bye is not a penalty or a judgment. The member remains in the next rotation.

### Meeting

The dyad happens wherever and however the two people arrange it. The Weave does not schedule the meeting, host the call, observe the encounter, or record the practice.

### Closing the loop

On Friday, each person receives a private check-in. They can say:

- We met.
- We have a time planned.
- We did not meet.

If they did not meet, they may name the obstacle or decline to say. They may also leave a private reflection or ask for steward support. Their partner never sees the response.

This check-in helps the stewards understand whether the service is working and where members are encountering friction. It does not rate either person, create a reliability score, or influence future matching.

## 3. The weekly rhythm

The current V1 rhythm is anchored to the Saturday Gathering. All times below are Eastern Time.

| Time | What happens |
|---|---|
| Saturday, 9:00 a.m. | The week's profile and standing cutoff. Changes made later may be held for the next cycle. |
| Saturday, 9:05 a.m. | The system prepares a draft: selected pairings first, then the automatic weave, then any byes. |
| Saturday, by noon | A steward reviews the pool, pairings, byes, and any exceptions, and either approves the cycle or revises it. |
| Saturday, 1:00–2:30 p.m. | The ARC Gathering. |
| Saturday, 3:15 p.m. | The approved pairing and bye emails are released. If no steward has approved the cycle, the system holds it. |
| Friday, noon | Each paired member receives the private check-in. |

The system never approves its own pairings. Automation prepares and sends an approved cycle; stewardship remains the release threshold.

## 4. Availability and eligibility

Members may enter up to two recurring availability windows per day, in half-hour increments. Each window must be at least one hour long. Availability is stored in the member's own time zone and translated safely across time zones and daylight-saving changes.

The member also chooses one of three flexibility settings:

- only the times entered;
- some flexibility beyond them;
- generally flexible.

Flexibility and private notes give stewards context, but the automatic matcher does not infer availability from them. Two members are eligible to be paired only when their entered windows contain at least one continuous hour of overlap in the relevant week.

This rule is intentionally strict: the Weave will not pair people who have no known overlapping availability. Greater availability therefore opens the possibility of meeting more of the network.

The system does not read anyone's calendar. The recurring windows are a coordination aid, not a reservation. The pair still confirms an actual time by replying to the email.

## 5. How the weave is made

The Weekly Weave is a deterministic batch process, not an AI recommendation system. Given the same member state and steward instructions, it produces the same draft.

### Hard conditions

The system will not pair two people when:

- either person is not active or has an incomplete routing profile;
- they do not share a continuous one-hour availability window; or
- a steward has recorded a private boundary that they must not be paired.

Private boundaries persist across weeks. A member does not need to justify a boundary to the system or to the other person.

### Steward-selected pairings

Before the automatic weave runs, a steward may select particular pairs for that week. This allows human intuition and knowledge of the network to shape the weave without turning the whole process into manual scheduling.

A selected pair must still satisfy the hard conditions above. The system does not override a private boundary or invent availability. Once selected, those members are removed from the automatic pool, and the rest of the network is woven around them. The introduction email does not reveal whether a pairing was selected or automatic.

### Automatic priorities

Among eligible pairings, the system applies these priorities in order:

1. Pair as many active members as possible.
2. Prefer encounters between people who have never been paired.
3. When repeats are necessary, prefer the pair that met least recently.
4. Reduce the chance that someone who recently received a bye receives another immediate bye.
5. Use the amount of shared availability as a secondary preference.
6. Resolve any remaining ties in a stable, repeatable way.

The network wants the network to meet itself. Novelty is therefore preferred, but it is not an absolute rule: at small scale or under tight availability, a repeat encounter may be better than no encounter.

### Odd numbers and constrained availability

With an odd number of eligible members, at least one person receives a bye. The same may happen with an even number if the availability pattern or private boundaries make a complete weave impossible. The system seeks the largest eligible set of pairs and uses recent bye history to distribute unmatched weeks more fairly.

## 6. Pausing and leaving

Every member receives a private profile link. Through it they can change their time zone, availability, or weekly standing without creating an account.

The standing states are:

- **Active:** included in the weekly pool.
- **Paused:** excluded until the member chooses to return.
- **Departed:** permanently removed from future routing by a steward.

A member who wants to step out for one week or a season pauses and later resumes. The V1 service does not maintain a separate vacation calendar or ask people to pass on each individual weave.

If a member pauses or changes relevant information after a draft has been made but before it is released, the old draft is no longer trusted. The steward must prepare and approve a fresh cycle.

A member who wants to leave the service can contact stewardship. Departure stops future routing and revokes active action links. It does not silently rewrite the historical fact that earlier pairings occurred.

## 7. When a weave does not become an encounter

The Weave does not watch the reply-all thread or infer whether a meeting happened. It learns only what members choose to report in the Friday check-in.

If the pair never schedules, each person can report that privately. The two accounts may differ; the system preserves both rather than forcing a shared verdict. A missed encounter does not automatically create a sanction, alter the matcher, or mark anyone as unreliable.

A steward may follow up when a member asks for support, when a pattern requires care, or when the operation of the service needs clarification. Feedback is treated as field intelligence for tending the practice and improving the service, not as a hidden reputation system.

## 8. Tending

The Weave is automated where repetition helps and human where judgment matters. A network steward tends it each week by:

- recording any member-requested private boundaries;
- adding any intentional pairings before the draft;
- reviewing who is in the pool and whether their profiles are complete;
- inspecting the proposed pairs, byes, and exceptions;
- rerunning the draft if member state has changed;
- approving the cycle for release;
- checking that the emails were delivered; and
- reviewing private check-ins and support requests with appropriate discretion.

Members can reach ARC stewardship from a support link included throughout the service and its emails. The support form goes to the shared ARC stewardship inbox rather than into the matching database. A member may write in text or, outside the form, use whatever ordinary contact method stewardship has made available. The normal aim is a response within forty-eight hours when a response is requested.

The current support route is an ordinary stewardship route. ARC has not yet established an independent safety or accountability channel, and the Weave does not present the existing route as one.

## 9. Data in service of the weave

The Weave keeps the minimum operational memory needed to route people responsibly and explain what it did.

### What it stores

- name and email address;
- time zone, recurring availability, and flexibility setting;
- an optional private availability note;
- active, paused, or departed standing;
- the version and time of required acknowledgments;
- pairing and bye history;
- weekly cycle drafts, approvals, and release state;
- email delivery state;
- the member's own check-in outcome;
- optional private feedback or support requests; and
- a limited audit trail of steward and system actions.

The routing data lives in a dedicated Weekly Weave database. ARC's membership record remains separate: joining the Weave does not make a person a member, and leaving the Weave does not by itself change their wider relationship to ARC.

### What another member sees

A matched member sees only what is necessary to coordinate:

- their partner's name and email address; and
- the mutual availability windows derived from both profiles, displayed in both time zones.

They do not see the other person's full availability, flexibility setting, private note, check-in, feedback, boundaries, pairing history, or whether a steward selected the pairing.

### What the Weave does not collect or infer

The Weave does not:

- read calendars or inboxes;
- ingest WhatsApp activity;
- observe, record, or transcribe encounters;
- build psychological or social profiles;
- score participation, reliability, compatibility, or value;
- track email opens or clicks; or
- use check-ins, feedback, or support requests as matching inputs.

### Access, links, and retention

Member action links are signed, purpose-specific, and time-limited. Steward functions require separate authentication. Sensitive configuration, the database, backups, and operational logs are restricted to the service and authorized stewards.

Data is retained by purpose rather than by an adopted universal deletion interval. Pausing does not erase history because repeat spacing and fair treatment of byes depend on it. After departure, the service may retain minimal historical pairing facts where deleting them would damage another member's record or the integrity of future routing. A member may ask for an explanation, export, correction, or deletion of data that is eligible to be removed.

The service-specific data policy is presented and affirmed inside the Weekly Weave because participation in the Weave is distinct from ARC membership and from any future ARC microservice.

## 10. Relationship to the rest of ARC

### ARC membership and onboarding

The Weekly Weave has its own enrollment and data-policy threshold. Its routing profile is not the source of truth for ARC membership. Membership is confirmed through ARC's wider onboarding and stewardship process.

### The Gathering

The Saturday Gathering anchors the weekly rhythm. Pairings are released after it, extending the shared field of the Gathering into one-to-one encounter during the week that follows. A member does not need to attend the Gathering to receive a weave unless ARC later adopts that as an explicit participation rule.

### WhatsApp

The ARC WhatsApp group is a separate social surface. The Weave has no WhatsApp settings, does not ingest group activity, and does not depend on WhatsApp for routing. Members may use whatever channel they mutually choose after the email introduction, but the designed coordination path is reply-all email.

### Steward support

Support is adjacent to the Weave but not part of the matcher. A member can report discomfort, ask for help, request a private no-pair boundary, correct their information, or leave the service without disclosing the request to a partner.

## 11. Scope

The Weave's scope is the weekly rotation, deliberately (D29). Other movements the network may want — additional practice beyond the weekly rhythm, offerings and gatherings surfaced, needs made visible — belong to possible future tools of the wider coordination layer. The *Source & Need Protocol* describes that direction rather than a present commitment.

The Weave stays small until member experience shows that another layer is necessary. New functions should arise from observed use, explicit requests, and steward learning, not from a desire to make the system appear complete in advance.

## 12. What it refuses

The Weave keeps no scores, streaks, ratings, or public participation counts. It does not simulate relationship, measure presence, gamify faithfulness, or decide who is a good member. It does not rank people by desirability, optimize for hidden traits, or turn private reflections into matching signals.

It does not automate consent away. Joining is a standing request to participate; pausing and private boundaries remain available at any time. Steward-selected pairings cannot override those boundaries or the basic requirement of shared availability.

It does not replace human judgment. Matching shapes who encounters whom — which is real power, and the reason the system stays legible, small, reviewable, and tended by people who are themselves inside the practice.

## 13. The ground

Matching is not an administrative function. It is the network's experiential threshold: for many members, the Weekly Weave email is where ARC's care becomes concrete. The encounter comes before the ideology. (*The Design Posture of the ARC*, “Matching as experiential proof.”)

The technical design follows from that ground:

- friction should be low;
- matching rules should be understandable;
- private information should remain private;
- automation should not conceal consequential judgment;
- feedback should improve the service without becoming surveillance; and
- the system should leave room for the network to teach its builders what it needs.

## 14. Implementation posture

V1 is a small standalone web service with a dedicated routing database, a scheduled weekly process, and transactional email delivery. Its public pages use ARC's paper-and-ink visual language. Members interact through ordinary web forms and email; there is no member account system and no general-purpose ARC app behind it.

The implementation is intentionally more modest than the possible coordination layer described elsewhere in the corpus. It is enough machinery to enroll members, find eligible pairs, preserve boundaries and history, support human review, send the weave, and hear what happened.

## 15. Known limits and open work

The following are acknowledged limits of V1, not hidden features or implied commitments:

- ARC has not yet adopted a fixed deletion schedule for every class of Weekly Weave data.
- The service has an ordinary steward-support route, not an independent safety or accountability channel.
- Availability is recurring rather than date-specific; one-off travel and exceptions are handled by pausing or updating the profile before the weekly cutoff.
- The Weave does not know whether a meeting occurred unless a member answers the private check-in.
- At small network size or under narrow availability, repeats and byes may be unavoidable.
- The effect of the matching priorities should be reviewed through real use, especially repeat spacing, bye distribution, and whether the stated availability model is sufficient.

These limits are reasons to tend and learn, not reasons to pre-build a larger platform. Any V2 change should answer a demonstrated member or steward need while preserving the service's legibility and restraint.

## 16. Lineage

The Weekly Weave is the survivor of a wide search: the Telegram routing bot (Phase 0, retired), the routing system V1 build plan (prototype, not launched), and the coordination-app designs (now proposals). Those documents remain in the corpus as gestures toward what the coordination layer might become.

The Weekly Weave is what ARC put live: the simplest service that could route members into regular dyadic practice while honoring availability, memory, private boundaries, and human stewardship.

---

*V1.0 — 2026-07-29. Daniel Thorson's description completed against the activated Weekly Weave build, its operating documentation, and the service-specific data policy.*
