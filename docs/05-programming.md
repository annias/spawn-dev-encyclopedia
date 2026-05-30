# GAME DEVELOPMENT LANGUAGE & CONCEPTS ENCYCLOPEDIA

## Chapter 5 — Programming & Technical Development Terminology

---

# The Core Mental Shift: What “Programming” Means in Games

In game development, programming is not just “writing code.”

Professionally, it is:

> The construction of real-time simulation systems that must remain stable, performant, and responsive under unpredictable user behavior and hardware constraints.

Game programming is fundamentally different from most software engineering because:

- Everything is real-time
- Everything is interactive
- Everything is performance-sensitive
- Everything is failure-visible (instantly to players)

A common AAA framing:

> “If backend software is about correctness, game code is about correctness under pressure.”

---

# Chapter 1: The Game Loop — The Heart of Everything

At the core of every game is the **game loop**.

## Game Loop

A repeating cycle that updates simulation every frame.

```
Input → Update → Simulation → Render → Repeat
```

This loop runs ~30–240 times per second depending on platform.

---

## Why it matters

Everything in a game exists inside this loop:

- Player movement
- AI behavior
- Physics
- Animation
- UI updates

If it is not in the loop, it is not “alive.”

---

## Frame

A single iteration of the game loop.

Professionals often say:

- “Frame spike”
- “Frame budget”
- “Frame time”

---

## Frame Time

How long one frame takes to compute.

Example:

- 16.6 ms → 60 FPS
- 33 ms → 30 FPS

---

## Tick

A simulation update step.

Sometimes decoupled from rendering.

---

## Delta Time

Time between frames.

Used to make movement consistent across frame rates.

---

# Chapter 2: Architecture Thinking (How Professionals Structure Code)

Game code is not written as a flat script.

It is structured into systems.

---

## System Architecture

A system is:

> A self-contained module that manages a domain of gameplay or engine behavior.

Examples:

- Physics system
- Animation system
- Input system
- AI system

---

## ECS (Entity Component System)

A modern architecture pattern.

### Entity

A unique ID.

No behavior.

---

### Component

Data only.

Example:

- Position
- Health
- Velocity

---

### System

Logic that operates on components.

Example:

- Movement system updates positions

---

### Why ECS exists

Traditional OOP struggles with:

- Performance
- Cache efficiency
- Large-scale simulation

ECS solves this by prioritizing:

> Data over hierarchy

---

## OOP (Object-Oriented Programming)

Classic model:

- Classes
- Inheritance
- Encapsulation

Used heavily in older engines and still common in gameplay code.

---

## Data-Oriented Design (DOD)

Design philosophy:

> Optimize for how data is accessed, not how objects are modeled.

Used in AAA engines for performance-critical systems.

---

## Composition over Inheritance

Modern principle:

> Build behavior from modular pieces instead of deep class trees.

---

# Chapter 3: Core Gameplay Programming Concepts

---

## State Machines

A system where behavior is defined by discrete states.

Example:

```
Idle → Walk → Run → Jump → Fall → Land
```

Used in:

- Characters
- AI
- UI flow
- Animation

---

## Finite State Machine (FSM)

A state machine with limited defined transitions.

---

## Event System

A system where actions trigger notifications.

Example:

- Player dies → event fires → UI updates → sound plays

Decouples systems.

---

## Observer Pattern

Design pattern used for event systems.

---

## Input System

Handles player control devices:

- Keyboard
- Mouse
- Gamepad

Modern systems separate:

- Raw input
- Action mapping
- Context-sensitive input

---

# Chapter 4: Physics Systems

---

## Physics Engine

Simulates:

- Gravity
- Collisions
- Forces
- Momentum

---

## Collision Detection

Determining when objects intersect.

Types:

- AABB (Axis-Aligned Bounding Box)
- Sphere collision
- Mesh collision

---

## Rigidbody

Object affected by physics simulation.

---

## Kinematic Object

Object moved manually, not by physics forces.

---

## Raycasting

Casting an invisible line to detect hits.

Used for:

- Shooting
- AI vision
- Interaction detection

---

## Hit Scan vs Projectile

### Hitscan

Instant hit detection.

Example: laser gun.

---

### Projectile

Physical object travels through space.

Example: bullet, arrow.

---

# Chapter 5: AI Programming Terminology

---

## Behavior Tree

Hierarchical AI decision system.

Structure:

- Selector nodes
- Sequence nodes
- Leaf actions

---

## Utility AI

AI chooses actions based on weighted scoring.

More dynamic than behavior trees.

---

## Pathfinding

Finding optimal route through space.

Most common algorithm:

### A* (A-Star)

---

## NavMesh (Navigation Mesh)

Precomputed walkable surfaces.

Used by AI agents.

---

## Steering Behaviors

Local movement rules:

- Seek
- Flee
- Avoid
- Wander

---

# Chapter 6: Performance Optimization (Critical AAA Discipline)

---

## Profiling

Measuring performance bottlenecks.

Tools show:

- CPU usage
- GPU usage
- Memory usage

---

## Bottleneck

The slowest part of a system limiting performance.

---

## CPU Bound

Limited by processing power.

---

## GPU Bound

Limited by rendering complexity.

---

## Draw Calls

Instructions sent to GPU to render objects.

Too many = performance issues.

---

## Batching

Combining multiple objects into fewer draw calls.

---

## Occlusion Culling

Not rendering objects hidden behind others.

---

## LOD (Level of Detail)

Using simpler models at distance.

Example:

- High-poly close
- Low-poly far

---

## Memory Management

Handling RAM usage efficiently.

Includes:

- Allocation
- Garbage collection
- Pooling

---

## Object Pooling

Reusing objects instead of creating/destroying them.

Used for:

- Bullets
- Particles
- Enemies

---

# Chapter 7: Networking (Multiplayer Systems)

---

## Client-Server Architecture

Most common multiplayer model.

### Client

Player machine.

### Server

Authoritative game state.

---

## Authority

Who decides truth.

In modern games:

> Server is usually authoritative.

---

## Peer-to-Peer (P2P)

Players connect directly.

Less common due to cheating and instability.

---

## Latency

Delay between action and response.

---

## Lag Compensation

Techniques to hide latency.

Examples:

- Hit rewinding
- Client prediction

---

## Client Prediction

Client assumes result before server confirms.

---

## Server Reconciliation

Correcting client when server disagrees.

---

## Replication

Synchronizing state across network.

---

## Tick Rate

How often server updates.

Higher tick rate = smoother gameplay but higher cost.

---

## Rollback Netcode

Used in fighting games.

System:

- Simulate future guesses
- Roll back if incorrect
- Recompute state

---

# Chapter 8: Engine Architecture Concepts

---

## Game Engine

Software framework providing:

- Rendering
- Physics
- Audio
- Input
- Tools

Examples:

- Unreal Engine
- Unity

---

## Middleware

External tools integrated into engine.

Examples:

- Physics engines
- Audio systems

---

## Scripting Layer

High-level gameplay logic layer.

Often uses:

- Lua
- C#
- Blueprints

---

## Rendering Pipeline

Sequence transforming 3D data into final image.

Stages:

- Geometry processing
- Lighting
- Rasterization
- Post-processing

---

# Chapter 9: Debugging Language (Professional Communication)

---

## Bug

Unexpected behavior.

---

## Repro Steps

Steps to consistently trigger a bug.

---

## Edge Case

Rare or extreme scenario.

---

## Crash

Program termination due to critical failure.

---

## Memory Leak

Memory not properly released.

---

## Null Reference

Missing object reference.

---

## Race Condition

Timing-dependent bug in concurrent systems.

---

# Chapter 10: Build Systems & Production Code Language

---

## Build

Compiled version of the game.

---

## Pipeline

Automated system turning code into playable builds.

---

## CI/CD (Continuous Integration / Deployment)

Automated testing and build generation.

---

## Version Control

Tracking code changes.

Common system:

- Git

---

## Merge Conflict

When two changes overlap.

---

## Branching

Parallel development streams.

---

# Chapter 11: Gameplay Programming vs Engine Programming

---

## Gameplay Programmer

Focus:

- Player behavior
- Mechanics
- Systems interaction

---

## Engine Programmer

Focus:

- Rendering
- Physics
- Performance
- Core architecture

---

## Tools Programmer

Focus:

- Editor tools
- Workflow optimization
- Production efficiency

---

## Technical Director (TD)

Focus:

> High-level technical vision and system architecture.

---

# Chapter 12: Senior-Level Programming Mental Models

---

## Systems Thinking

Understanding how components interact as a whole.

---

## Determinism

Same input → same output.

Important for:

- Multiplayer
- Replays

---

## Emergent Complexity

Simple rules producing complex behavior.

---

## Abstraction Layers

Separating complexity into levels.

Example:

- Input layer
- Gameplay layer
- Engine layer

---

## Performance Budgeting

Allocating CPU/GPU cost across systems.

Example:

- 5 ms AI
- 6 ms rendering
- 2 ms physics

---

# Key Insight

Beginners think:

> “How do I make this feature work?”

Intermediate programmers think:

> “How do I structure this system cleanly?”

Senior engineers think:

> “How do I design systems that remain stable, scalable, and debuggable under real-time constraints?”

Expert engineers think:

> “How do I model simulation truth across CPU, GPU, network, and player perception simultaneously?”