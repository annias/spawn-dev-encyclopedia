# GAME DEVELOPMENT LANGUAGE & CONCEPTS ENCYCLOPEDIA

## Chapter 6 — Audio Development Vocabulary

---

# The Core Mental Shift: What “Audio” Means in Games

In games, audio is not decoration.

It is:

> A real-time feedback, emotion, and information system that operates in parallel with visuals and gameplay mechanics.

In professional terms:

- Visuals show what is happening
- Gameplay defines what is happening
- Audio tells you how it _feels_ and often what to _pay attention to first_

A common AAA insight:

> “Players forgive visual confusion before they forgive audio confusion.”

Because sound is often the fastest communication channel in games.

---

# Chapter 1: The Three Functions of Game Audio

Every sound in a game typically serves at least one of three roles:

---

## 1. Informational Audio

Audio that communicates gameplay state.

Examples:

- Low health warning
- Enemy nearby
- Objective complete
- Reload click

This is often called:

> **Feedback audio**

---

## 2. Emotional Audio

Audio that shapes mood.

Examples:

- Ambient wind in horror games
- Orchestral tension buildup
- Peaceful environmental music

This is often called:

> **Atmospheric audio**

---

## 3. Mechanical Audio

Audio tied directly to player actions.

Examples:

- Footsteps
- Gunshots
- Jump sounds
- UI clicks

This is often called:

> **Diegetic action feedback**

---

# Chapter 2: Core Sound Design Vocabulary

---

## Sound Design

The creation and shaping of audio assets for gameplay and emotion.

Not just recording sounds, but:

- Layering
- Processing
- Timing
- Contextual triggering

---

## Foley

Re-recording real-world actions in a studio.

Examples:

- Footsteps
- Cloth movement
- Object handling

Named after early film sound pioneer Jack Foley.

---

## SFX (Sound Effects)

General term for non-music audio assets.

Includes:

- Weapons
- UI sounds
- Impacts
- Environmental sounds

---

## One-Shot Sound

A sound that plays fully once.

Example:

- Gunshot
- Door slam

---

## Loop

A sound that repeats continuously.

Example:

- Engine hum
- Wind ambience

---

## Layering

Combining multiple sounds into one composite sound.

Example:

A gunshot may include:

- Trigger click
- Explosion
- Mechanical echo
- Sub-bass impact

---

## Transient

The initial attack portion of a sound.

Critical for:

> Perceived impact and responsiveness

---

## Tail

The decay portion of a sound.

Example:

- Reverb
- Echo
- Fade-out

---

# Chapter 3: Adaptive / Interactive Audio

---

## Adaptive Audio

Audio that changes dynamically based on game state.

Example:

- Combat music intensifies when enemies appear
- Calm music returns when safe

---

## Interactive Music

Music that responds to gameplay input or events.

Example:

- Adding percussion during combat
- Removing layers during stealth

---

## Stingers

Short musical cues triggered by events.

Example:

- Enemy spotted
- Boss phase change

---

## Music Layering System

Music broken into layers:

- Base layer (ambient)
- Tension layer
- Combat layer
- Boss layer

System dynamically mixes them.

---

## Vertical Re-Orchestration

Changing arrangement instead of just intensity.

Example:

Same melody, different instrumentation during combat.

---

## Horizontal Re-Sequencing

Switching between different musical sections.

Example:

Exploration → combat → victory themes.

---

# Chapter 4: Spatial Audio Vocabulary

---

## Spatial Audio

Audio positioned in 3D space relative to player.

Enables:

- Directionality
- Distance perception
- Environmental realism

---

## 3D Audio Source

Sound emitted from a point in world space.

Example:

Enemy footsteps behind player.

---

## Attenuation

Reduction of volume over distance.

---

## Occlusion

Sound being blocked by objects.

Example:

Sound muffled behind a wall.

---

## Reverb

Echo effect based on environment.

Examples:

- Cave → long reverb
- Room → short reverb
- Outdoors → minimal reverb

---

## HRTF (Head-Related Transfer Function)

Mathematical model simulating how human ears perceive direction.

Used in:

- VR audio
- 3D headphone sound

---

# Chapter 5: Audio Middleware (Production Systems Layer)

---

## Audio Middleware

External systems that manage game audio logic.

Used because engines alone are often too limited.

Common tools:

- FMOD
- Wwise

---

## Event-Based Audio System

Audio triggered by events rather than hardcoded calls.

Example:

```
Player jumps → event triggers → sound system plays jump sound
```

This decouples audio from gameplay code.

---

## Audio Events

Named triggers for sound playback.

Example:

- Play_Explosion_Large
- Play_UI_Click
- Play_Enemy_Spawn

---

## Parameter-Based Audio

Audio changes based on variables.

Examples:

- Speed affects engine pitch
- Health affects heartbeat intensity

---

## RTPC (Real-Time Parameter Control)

Used in Wwise.

Allows continuous audio modulation.

Example:

- Danger level → music intensity

---

# Chapter 6: Mixing & Mastering Vocabulary

---

## Mixing

Balancing all audio elements together.

Includes:

- Volume balance
- Frequency separation
- Spatial placement

---

## Mastering

Final audio processing step.

Ensures:

- Consistency
- Loudness standards
- Platform compliance

---

## Dynamic Range

Difference between quiet and loud sounds.

---

## Compression (Audio)

Reducing dynamic range.

Used to:

- Make sounds more consistent
- Improve clarity in gameplay

---

## EQ (Equalization)

Adjusting frequency balance.

Example:

- Removing bass muddiness
- Enhancing clarity

---

## Loudness Normalization

Ensuring consistent perceived volume.

Important for:

- Consoles
- Streaming platforms

---

# Chapter 7: Psychological Function of Audio

---

## Audio Feedback Loop

Audio confirms player actions.

Example:

- Shooting → gun sound → hit marker sound

This reinforces:

> Agency and responsiveness

---

## Auditory Masking

When one sound hides another.

Example:

Explosion masking footsteps.

---

## Audio Hierarchy

Prioritizing important sounds.

Example:

- Enemy attack > ambient wind > UI click

---

## Cognitive Load Reduction

Good audio reduces need for visual attention.

Example:

You hear enemy behind you before seeing them.

---

## Pavlovian Audio Design

Conditioned responses through repetition.

Example:

- Loot sound = reward dopamine trigger

Used heavily in:

- Loot games
- Live service games

---

# Chapter 8: Genre-Specific Audio Language

---

## FPS Audio

Focus:

- Positional accuracy
- Weapon clarity
- Tactical feedback

Key terms:

- Footstep occlusion
- Weapon tail clarity
- Distance attenuation

---

## Horror Audio

Focus:

- Ambiguity
- Unease
- Absence of sound

Key concepts:

- Silence design
- Sub-bass tension
- Unresolved audio cues

---

## RPG Audio

Focus:

- Emotional atmosphere
- World immersion
- Long-form ambience

---

## Multiplayer Audio

Focus:

- Competitive clarity
- Fast recognition
- Priority sounds

---

## Mobile Audio

Focus:

- Compression
- Clarity on speakers
- Battery-friendly processing

---

# Chapter 9: Technical Audio Systems

---

## Audio Engine

System that processes and plays sound.

---

## Voice Limiting

Limiting number of simultaneous sounds.

Prevents audio overload.

---

## Audio Pooling

Reusing audio instances for performance.

---

## Streaming Audio

Loading long sounds dynamically.

Example:

Music tracks, cutscenes.

---

## Sample Rate

How many audio samples per second.

Higher = better quality, more cost.

---

## Bit Depth

Resolution of audio amplitude.

Affects dynamic range quality.

---

# Chapter 10: Audio Programming Concepts

---

## Audio Thread

Separate processing thread for sound.

Prevents blocking gameplay loop.

---

## Latency

Delay between trigger and playback.

Critical for responsiveness.

---

## Audio Tick

Regular update cycle for audio system.

---

## Event Queue

System storing pending audio events.

---

# Chapter 11: Cross-Disciplinary Communication (Audio Language)

---

## Designers → Audio Team

Instead of:

> “Make it sound cool”

They say:

- “This attack needs stronger telegraphing”
- “We need clearer hit confirmation”
- “This area should feel unsafe audibly”

---

## Programmers → Audio Team

Instead of:

> “Play sound here”

They say:

- “Trigger event on state change”
- “Expose parameter for intensity scaling”

---

## Artists → Audio Team

Instead of:

> “This should feel scary”

They say:

- “We want low-frequency rumble here”
- “Space feels enclosed visually, audio should reinforce that”

---

## Audio Director Role

Responsible for:

- Overall sound identity
- Consistency across systems
- Emotional alignment
- Mixing standards

Not just sound creation — sound strategy.

---

# Chapter 12: Senior-Level Audio Mental Model

Beginners think:

> “What sound should this object make?”

Intermediate developers think:

> “How do I make this sound realistic?”

Senior audio designers think:

> “What information, emotion, and feedback should this sound communicate within the player’s cognitive load?”

Expert audio designers think:

> “How does sound shape player attention, reaction timing, emotional state, and perceived responsiveness in real time?”

---

# Key Insight

In high-level game development:

> Audio is not an effect. It is a communication channel faster than vision.