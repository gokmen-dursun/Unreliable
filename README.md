# Unreliable
> Everyone tells the truth, not everyone knows it.

Hi, I'm Gokmen Dursun, from Lyon, France. Unreliable is a multiplayer social deduction game I'm building from scratch while learning to code, as the centerpiece of my Ivy League application and my first real engineering project.

## The Concept

Unreliable is a multiplayer social game for 5 to 10 players. Everyone gathers in a closed location — a café, a common room — and a mysterious incident occurs. An object disappears. Something happens that nobody fully saw.

Each player receives a personal clue about what happened. But here's the twist: **some clues are subtly false, and no player knows whether their own clue is reliable or not.**

Players explore the location, interact with objects to gather more information, and discuss with each other to piece together the truth. Then comes a collective vote — and the final revelation shows who was right, who was wrong in good faith, and who the real culprit was all along.

## What Makes It Different

In most social deduction games like Among Us, lying is an **active choice**. You know you're lying and your opponents know someone is lying.

In Unreliable, **the confusion is built into the system itself.** An innocent player can convince the entire group of a false theory — not because they're bluffing, but because they genuinely believed what they said. Their clue was wrong, but they never knew.

The question isn't *"who is lying?"* It's *"who is right?"* — and that's a fundamentally harder question to answer.

## The Core Technical Challenge

The game runs on a **server-authoritative architecture with asymmetric information distribution.** The server is the only entity that knows the full truth and it sends each player a different version of reality — and it must never leak one player's clues to another client, or the entire game breaks.

This is a real distributed systems problem: managing trust, authority, and partial information across multiple clients in real time. Solving it cleanly is what this project is really about.

**Key problems to solve:**
- Server authority and cheat prevention — clients never receive what they're not supposed to know
- Real-time state synchronization across players
- Procedural incident and clue generation with controlled false information
- Synchronized voting system with simultaneous reveal

## Built With

| Technology | Role |
|---|---|
| Unity | Game engine |
| C# | Programming language (learning from scratch) |
| Photon Fusion / NGO | Multiplayer networking (TBD) |
| GitHub | Full transparency on the build journey |

## The Roadmap

| Phase | Description | Timeline |
|---|---|---|
| 1 | Learn C# fundamentals | Jul → Oct 2026 |
| 2 | Learn Unity basics, build first solo game | Jul → Oct 2026 |
| 3 | Learn multiplayer networking on a minimal prototype | Nov 2026 → Feb 2027 |
| 4 | Build Unreliable V0 — core mechanics, grey-box | Mar → May 2027 |
| 5 | Build Unreliable MVP++ — playable, documented, presentable | Jun → Oct 2027 |

## Why This Project

I want to study software or embedded systems engineering at an Ivy League university. I could have built a to-do app or a clone of an existing game. Instead I chose a problem I haven't seen solved the way I want to solve it — and a technical challenge that forces me to understand distributed systems, network architecture, and real-time synchronization from the ground up.

The goal isn't to ship a commercial game. The goal is to prove I can identify a hard problem, break it down, and build my way through it — documented commit by commit.

## Project Info

| | |
|---|---|
| Type | Multiplayer PC game |
| Engine | Unity (C#) |
| Status | Learning phase — started July 2026 |
| Target | MVP++ by October 2027 |
| Cost | Around 30-50$ |

## Author

**Gokmen Dursun** — Lyon, France

I'm not a developer yet but I'm learning as I build. Every commit on this repo is proof that you don't need to wait until you're ready but you just need a problem worth solving.

📍 Lyon, France — building since July 2026
