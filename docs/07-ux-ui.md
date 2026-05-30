# GAME DEVELOPMENT LANGUAGE & CONCEPTS ENCYCLOPEDIA

## Chapter 7 — UX & UI (User Experience & User Interface Terminology)

---

# The Core Mental Shift: What UX/UI Means in Games

In games, UX/UI is not “menus and HUDs.”

Professionally, it is:

> The system that translates complex simulation state into human-readable, actionable information under real-time pressure.

A strong AAA principle:

> “If the player is confused, the UI has failed — even if the system is working perfectly.”

UX/UI is fundamentally about:

- Clarity
- Decision support
- Cognitive load management
- Attention guidance
- Interaction speed

---

# Chapter 1: UX vs UI (Critical Distinction)

These terms are often confused.

---

## UI (User Interface)

The **visual and interactive layer**.

Examples:

- HUD
- Menus
- Buttons
- Icons
- Maps

UI is what the player sees and interacts with.

---

## UX (User Experience)

The **total experience of interacting with the game systems**.

Includes:

- Navigation flow
- Menu friction
- Clarity of systems
- Tutorial effectiveness
- Feedback timing

UX exists even without visible UI.

Example:

- Movement feel = UX
- Inventory frustration = UX
- Confusing quest flow = UX

---

# Chapter 2: Information Architecture (IA)

---

## Information Architecture

The structural organization of information.

In games:

> How systems are grouped, labeled, and accessed.

Examples:

- Inventory → Equipment → Crafting
- Main menu → Settings → Audio → Controls

---

## Why IA matters

Poor IA causes:

- Player frustration
- Feature invisibility
- Cognitive overload

Good IA makes complexity feel simple.

---

# Chapter 3: Cognitive Load (Core UX Concept)

---

## Cognitive Load

The amount of mental effort required to understand a system.

---

## Types of Cognitive Load

### Intrinsic Load

The natural complexity of the system.

Example:

Learning chess rules.

---

### Extraneous Load

Unnecessary confusion caused by poor design.

Example:

Bad UI layout.

---

### Germane Load

Useful mental effort that builds mastery.

Example:

Learning combat systems over time.

---

# UX Goal:

> Minimize extraneous load while preserving meaningful intrinsic load.

---

# Chapter 4: Interaction Design (IxD)

---

## Interaction Design

How players interact with systems.

Focus:

- Inputs
- Responses
- Feedback loops

---

## Input Mapping

Mapping controls to actions.

Example:

- A = Jump
- RT = Shoot

---

## Responsiveness

How quickly the game reacts to input.

Critical concept:

> “Input delay breaks immersion more than visual quality issues.”

---

## Feedback Timing

Time between action and response.

Examples:

- Hit confirmation sound
- Animation response
- UI flash

---

# Chapter 5: HUD (Heads-Up Display)

---

## HUD

On-screen overlay showing game state.

Examples:

- Health bar
- Ammo count
- Objective tracker

---

## Diegetic UI

UI existing within the game world.

Example:

- Health shown on character suit (Dead Space style)

---

## Non-Diegetic UI

Traditional overlay UI.

Example:

- Floating minimap
- Ammo counters

---

## Meta UI

Out-of-world systems.

Example:

- Pause menus
- Settings screens

---

# Chapter 6: Visual Hierarchy (Critical UI Skill)

---

## Visual Hierarchy

The order in which the eye processes information.

Controlled through:

- Size
- Contrast
- Color
- Position
- Motion

---

## Primary Information

What must be seen immediately.

Examples:

- Low health warning
- Enemy indicators

---

## Secondary Information

Supporting data.

Examples:

- Ammo
- Mini-map details

---

## Tertiary Information

Optional or contextual data.

Examples:

- Flavor text
- Lore descriptions

---

# Chapter 7: Affordance in UI

---

## UI Affordance

How an element suggests interaction.

Examples:

- Buttons look pressable
- Sliders look draggable
- Icons suggest function

---

## Signifiers

Visual cues that indicate interaction.

Example:

- Highlight on hover
- Glow on selection

---

## False Affordance

UI element looks interactive but is not.

This is a major UX failure.

---

# Chapter 8: Usability Testing

---

## Usability Testing

Observing real players interacting with the game.

Goal:

Identify confusion without developer bias.

---

## Heatmaps

Visual data showing where players look or click.

Used in:

- UI optimization
- Tutorial design

---

## Playtesting

Structured gameplay observation.

Key questions:

- Where do players get stuck?
- What do they misunderstand?
- What do they ignore?

---

## Telemetry

Quantitative behavioral data.

Examples:

- Time spent in menus
- Death locations
- Drop-off points

---

# Chapter 9: Accessibility (Modern AAA Requirement)

---

## Accessibility

Designing systems usable by players with disabilities.

Includes:

- Visual accessibility
- Audio accessibility
- Motor accessibility
- Cognitive accessibility

---

## Colorblind Modes

Adjusting UI color palettes for visibility.

---

## Subtitles

Text representation of audio.

Includes:

- Speaker labels
- Sound descriptions

---

## Input Remapping

Allowing players to customize controls.

---

## Difficulty Accessibility

Adjustable challenge systems.

---

# Chapter 10: UI Systems Vocabulary

---

## UI Framework

System that renders UI elements.

---

## Widget

Individual UI element.

Examples:

- Health bar widget
- Inventory slot widget

---

## Layout System

Rules controlling UI positioning.

---

## Anchoring

UI positioning relative to screen edges.

---

## Scaling

Adjusting UI size for resolution.

---

# Chapter 11: Navigation UX

---

## Menu Flow

How players move through UI screens.

---

## Friction

Anything slowing interaction unnecessarily.

Example:

Too many confirmation screens.

---

## Click Depth

Number of steps required to reach a function.

Lower = better UX.

---

## Dead Ends

Menus with no clear return path.

---

# Chapter 12: Feedback Systems

---

## Feedback Loop

System response to player actions.

Includes:

- Visual feedback
- Audio feedback
- Haptic feedback

---

## Haptics

Controller vibration feedback.

Used for:

- Impact
- Alerts
- Environmental effects

---

## Confirmation Feedback

Signals that action succeeded.

Examples:

- Button highlight
- Sound cue
- Animation response

---

## Error Feedback

Indicates invalid actions.

Examples:

- Red flash
- Error sound
- Shake animation

---

# Chapter 13: UX for Gameplay Systems

---

## Onboarding

Teaching players systems gradually.

---

## Progressive Disclosure

Revealing complexity over time.

Example:

New mechanics introduced slowly.

---

## Tutorialization

Explicit teaching moments.

---

## Soft Tutorial

Learning through gameplay rather than instructions.

Example:

Level design teaches mechanics implicitly.

---

# Chapter 14: UX Metrics

---

## Retention UX

How UX affects player return rates.

---

## Time to Fun

Time until player engages with core gameplay.

Critical KPI in modern design.

---

## Drop-off Rate

Where players quit.

---

## Engagement Friction

Points where players hesitate or disengage.

---

# Chapter 15: Genre-Specific UX Language

---

## FPS UX

Focus:

- Combat readability
- Crosshair clarity
- Enemy visibility

---

## RPG UX

Focus:

- Inventory management
- Skill trees
- Quest tracking

---

## Strategy UX

Focus:

- Information density
- Unit control systems
- Minimap clarity

---

## Mobile UX

Focus:

- Touch accuracy
- One-handed usability
- Session length optimization

---

# Chapter 16: Senior-Level UX Mental Model

---

## Beginner Thinking

> “How do we display this information?”

---

## Intermediate Thinking

> “How do we organize this interface?”

---

## Senior Thinking

> “How do we reduce cognitive load while preserving system depth and player agency?”

---

## Expert Thinking

> “How do we design information systems that allow players to make correct decisions under time pressure without consciously processing all available data?”

---

# Key Insight

In professional game development:

> UX is not about showing information. It is about controlling what the player _understands in time to act on it._