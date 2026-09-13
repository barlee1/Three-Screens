# Three Screens — Design Rationale

A prototype to help ward building reps track church cleaning assignments across wards, so tasks don't fall through the cracks between weeks.

## 1. Need, Persona, Capability, Value

| Question | Answer |
|---|---|
| **Need** | It's hard to know who is cleaning what, or when responsibility switches between wards. Ownership is unclear, monthly tasks get missed, and stake leaders have no way to confirm a task actually got done. Existing checklists don't capture completion. |
| **Persona** | Building reps for wards with high turnover. |
| **Capability** | The app lets them clean the church effectively by clearly showing what needs to be done, right now, in one place. |
| **Value** | The church is properly cleaned, and everyone helping feels certain about *how* to help — reducing wasted effort and uncertainty. |

*(Need, capability, and value are kept distinct: need is the frustration/workaround, capability is the observable action the app enables, value is the material/emotional payoff afterward.)*

## 2. The Three Screens

| Screen | Single Job | Why It Earned a Slot | Design Question It Explores |
|---|---|---|---|
| **1. Landing** | Signal "this app is for church cleaning" and route straight to today's cleaning list. Shows a small preview of unassigned tasks below. | Establishes *who* the app is for and *what* they can immediately do. | Persona & Capability |
| **2. Cleaning List** | Show every cleaning area and whether someone is already working on it today. | Lets anyone who shows up — even late — find open work without asking around. Keeps ward members accountable for tracking their own progress. | Need & Value |
| **3. Task Breakdown** | Show the specific tasks for one area, with overdue monthly tasks clearly flagged. | Ensures nothing gets silently skipped; if a ward runs out of time, the leftover tasks are visible and can be picked up next week. | Need & Value |

## 3. Design Question Plan

| Category | Interview Question | What I Learned | Basis |
|---|---|---|---|
| **Need** | "Tell me about the last time you were in this situation. What did you end up doing?" | As a building rep, I found tasks previous wards had missed and ended up doing 3–4 hours of extra cleaning myself just to cover the gaps. | Personal experience |
| **Value** | "What would have to be true for you to use a different solution instead of what you do now?" | It would need to be easy enough that *every* ward using the building actually logs their work when it's their turn. | Personal experience, knowledge of shared-building use |
| **Persona** | "What have you already tried?" | Manually re-checking every room and doing extra cleaning myself rather than trusting the existing checklist. | Personal experience |
| **Capability** | "What would you click/tap first, and what do you expect would happen?" | I'd tap "Today's Cleaning" and expect a full list of what needs cleaning to appear. | Landing screen currently has almost nothing else on it besides that one button. |

## 4. Design Justification & First Read

Opening the live URL cold, as a first-time user:

- **Does the landing screen signal the primary capability and value at first glance?**
 Not clearly enough — there was too much on the screen initially to tell at a glance what the app was for.

- **Does every element earn its place?**
 No. Multiple elements competed for attention, and the primary job (get to today's list) got lost in the clutter.

- **What belongs together, and which Gestalt principle explains it?**
 Tasks should be grouped by status — *done*, *needs doing*, *unassigned* — and **proximity** is the grouping principle that best communicates this.

- **Do screens 2 and 3 stay on mission, and can I get back to the landing screen from anywhere?**
 The screens stay on-mission, but navigation was broken — there was no way back to the home screen. That's a fix still needed. The screens themselves could also be simplified and reorganized around proximity grouping.

- **What did the AI initially get wrong, skip, or oversimplify?**
 The first draft packed too much information onto every screen, making it hard to tell what each screen's actual job was. I stripped each screen down so its one primary job could stand out.

- **Which design question or principle motivated each change?**
 **Proximity** was the main driver — grouping tasks by status instead of scattering related info. I also unified colors across all three screens so the app felt cohesive rather than three disconnected pages.

### Before / After: Landing Screen

| Before | After |
|---|---|
| <img width="390" alt="Before" src="https://github.com/user-attachments/assets/58023f2b-9b6b-4dd1-8ac6-02b952cc2ae5" /> | <img width="402" alt="After" src="https://github.com/user-attachments/assets/216a4413-4528-4c3a-81e4-4ee4383f2a9a" /> |
| No clear capability defined — the "today's cleaning" action competed with several other elements for attention, so nothing signaled the primary job. | Removed competing elements and shrank the "not yet assigned" list so it's visible but doesn't compete with the primary action. The single button now clearly signals the capability. |
