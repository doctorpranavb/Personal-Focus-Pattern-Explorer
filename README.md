# Personal Focus Pattern Explorer

### Time-of-day behavioral visualization for sustained USMLE preparation

*RescueTime API integration · productivity-pattern interpretation · AI-assisted software development*

> **Portfolio case study. Source code, scoring logic, thresholds, weighting, and detailed implementation are intentionally private.**

I built **Personal Focus Pattern Explorer** during dedicated USMLE preparation to transform my own computer-activity history into a visual picture of **when sustained focused work tended to occur — and when weaker or more interrupted patterns tended to take over**.

I was already using RescueTime to measure activity and distraction-blocking tools to protect study time. What I still lacked was an **interpretation layer**:

> **Which parts of my day consistently supported sustained, focused work, and which did not?**

<p align="center">
  <img src="media/02_focus-pattern-explorer_main-view_portfolio.png" width="100%" alt="Personal Focus Pattern Explorer time-of-day pattern view">
  <br>
  <sub><b>Selected time-of-day view comparing recent behavior with longer-term personal patterns. The original interface used the internal working title “Focus Zones.”</b></sub>
</p>

> Screenshots reflect my own real study data rather than demonstration content. Detailed scoring and interpretation logic are intentionally not shown.

---

## At a Glance

- **Time-of-day visualization** — converts activity history into an immediately readable hourly view
- **Current vs. historical comparison** — places recent behavior beside longer-term personal baselines
- **Continuity-aware interpretation** — distinguishes sustained productive activity from highly interrupted work
- **Visual trend cues** — makes recurring stronger and weaker periods easier to recognize
- **Real study use** — developed and repeatedly refined during dedicated USMLE preparation
- **Private implementation** — scoring, thresholds, weighting, and detailed interpretation logic remain unpublished

---

# From Measurement to Interpretation

During USMLE preparation, I was already using **RescueTime** to record computer activity and classify productive and distracting behavior.

I also used tools such as **Cold Turkey** and **Micro Manager** to restrict distractions during dedicated study periods.

That gave me two useful layers:

**Measurement** — RescueTime showed what happened.  
**Enforcement** — blocking tools helped prevent behaviors I wanted to avoid.  
**Interpretation** — this project helped me understand recurring patterns in the behavior I actually produced.

The tool uses my own RescueTime activity data to build a comparative, hour-by-hour representation of time-of-day patterns.

It was designed to make several questions easier to answer:

- At what times of day was focused work most consistent?
- Was today's pattern similar to or different from my longer-term history?
- Which periods appeared worth actively protecting from distraction?
- Were apparently productive hours actually sustained, or repeatedly interrupted?

One idea became especially important during development:

> **Productive time and focused time are not always the same thing.**

A long period inside applications classified as productive can still be highly fragmented by frequent context switching. The system therefore considers **continuity alongside productive activity**, rather than relying only on raw duration.

The goal is not to claim that the software measures biological circadian rhythm, cognition, psychological flow, or validated attention.

It visualizes **patterns in recorded computer-use behavior** as a practical aid for personal reflection and study planning.

---

## Used Inside the Real Study Environment

<p align="center">
  <img src="media/01_focus-pattern-explorer_panel-in-context_portfolio.png" width="100%" alt="Focus pattern mini-view operating inside an active USMLE study workflow">
  <br>
  <sub><b>The compact pattern view running alongside my actual Q-bank study workflow. Proprietary educational content has been intentionally obscured.</b></sub>
</p>

A compact view allowed the visualization to remain available during study rather than requiring me to leave the task and open a separate analytics dashboard.

That mattered because the useful moment was often not at the end of the week.

It was **before deciding how to use the next few hours**.

---

## What the Visualization Tries to Surface

At a high level, the interface helps reveal:

- **Recurring stronger periods** — hours where productive behavior remained comparatively consistent
- **Recurring weaker periods** — time blocks repeatedly associated with lower continuity or more distracting activity
- **Current vs. historical behavior** — whether today's pattern resembles or diverges from longer-term trends
- **Changing patterns over time** — whether particular parts of the day appear to be strengthening or weakening
- **Fragmentation** — whether apparently productive time was sustained or repeatedly interrupted

The public screenshots show the **output layer** only.

The scoring model, thresholds, historical weighting, confidence logic, fragmentation calculations, and detailed interpretation rules remain private.

---

<details>
<summary><strong>Development Progression & Technical Notes</strong></summary>

<br>

### Development progression

The project evolved gradually through real use rather than from a fixed specification.

**Early visualization**  
The first goal was simply to make hourly activity patterns easier to see.

**Historical comparison**  
Single-day data was not enough, so recent behavior was placed beside longer-term personal patterns.

**Continuity and fragmentation**  
Raw productive duration was supplemented by an interpretation of whether work appeared sustained or repeatedly interrupted.

**Visual refinement**  
Color, emphasis, compact views, and comparative states were repeatedly adjusted so patterns could be understood quickly.

**Reliability and edge cases**  
Daily use exposed issues involving asynchronous data loading, rendering order, state handling, precision, navigation, and interface behavior. These were repeatedly corrected as the tool matured.

The source went through **dozens of revisions**, many driven by problems that only became visible during everyday use.

### Technical snapshot

| Aspect | Detail |
| --- | --- |
| **Platform** | Browser-based JavaScript userscript |
| **Data source** | RescueTime API using my own activity data |
| **Interface** | Compact and expanded visualization views |
| **Core purpose** | Time-of-day behavioral pattern interpretation |
| **Development approach** | AI-assisted implementation with repeated real-world testing |
| **Source availability** | Private |

Detailed architecture, formulas, thresholds, weighting, caching structures, API handling, and classification logic are intentionally omitted.

</details>

---

## AI-Assisted Development

I did not hand-code the entire application from scratch.

I identified the problem, defined the desired behavior and interface, specified the comparisons and constraints, and used **AI-assisted implementation** to generate and revise the software.

I then repeatedly tested the tool against my own real RescueTime data, identified failures and edge cases, directed debugging, and validated revisions through continued use.

My role centered on:

**problem identification → concept design → specification → AI-assisted implementation → testing → failure detection → debugging direction → validation → refinement**

The exact model orchestration, prompts, handoffs, and development workflow are intentionally private.

What I am showcasing is the process of turning a personal behavioral problem into a working analytical tool through **system thinking, AI-assisted development, testing, debugging, and sustained refinement**.

---

## Current Limitations

This is a **personal exploratory tool**, not a validated productivity, cognitive, psychological, or chronobiological instrument.

Its output depends on the quality of the underlying RescueTime data and classifications.

It cannot determine:

- whether I truly understood what I was studying,
- whether a productive application was being used effectively,
- whether a period represented psychological flow,
- or whether a time-of-day pattern reflects an underlying biological rhythm.

The visualization should therefore be interpreted as a **behavioral signal for personal reflection**, not as an objective measure of cognitive performance.

---

## Project Status

**Personal-use analytics tool / portfolio case study**

The working source code, scoring model, thresholds, weighting system, detailed interpretation logic, and implementation architecture remain private.

This repository is intended to demonstrate the project's **purpose, interface, reasoning, development process, and real-world use** without publishing the information required to reproduce it.

---

## Author

**Pranav Krishna Buddhapuram**

Orthopaedic surgeon with interests in medical education, research, productivity systems, behavioral analytics, and practical AI-assisted software development.

GitHub: [@doctorpranavb](https://github.com/doctorpranavb)

---

## Intellectual Property

© 2026 Pranav Krishna Buddhapuram. All rights reserved.

This repository is a portfolio showcase only. No license is granted for copying, reproducing, redistributing, modifying, reverse-engineering, derivative implementation, or commercial use.

This is an independent personal project built using my own RescueTime activity data and API access. RescueTime provides the underlying activity-tracking data; this project is my independent interpretation and visualization layer.

It is **not affiliated with, sponsored by, or endorsed by RescueTime, Cold Turkey, Micro Manager, or any other third-party service mentioned.**
