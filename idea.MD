# Mini Golf Watch Game — Design Brief

## Overview

A single-player mini golf game for Apple Watch with a calm, tactile feel and a beautiful hand-drawn aesthetic. The game combines satisfying physics, progressive level design, and on-watch customization.

## Core Gameplay

### Shot Mechanic
- **Slingshot aiming**: Drag your finger away from the ball in the opposite direction you want it to go. The further you drag, the more power.
- **Feedback**: Haptic pulses on release; ball rolls with weight and momentum.
- **Feel**: Tactile and direct — the ball should feel like it has real mass.

### Physics
- Ball rolls smoothly across the fairway with realistic momentum and friction.
- Bounces off walls with satisfying impact feedback — different haptics for soft vs. hard collisions.
- Cup mechanics: slow enough to sink gently, fast enough to lip out and roll back.
- Obstacles interact predictably: push the ball, slow it, or redirect it.

### Per-Hole Loop
1. Tee off with aim preview
2. Roll the ball toward the cup
3. See result (stroke count vs. par) after sinking
4. Move to next hole
5. See full round scorecard with best round tracking

## Visual Style

### Perspective
- Bird's-eye view tilted toward the horizon (pseudo-3D perspective).
- Camera follows the ball smoothly as it rolls down the fairway.
- Larger courses scroll off-screen; the camera pans naturally to keep the ball visible.

### Color & Design
- **Fairway**: Soft muted green (the main playing surface).
- **Walls**: Warm gray sides with crisp white tops — looks 3D and solid.
- **Ball**: Off-white with soft shading, sits on top of the fairway.
- **Outlines**: Thin dark lines where walls meet the fairway — crisp, clean look.
- **Accents**: Flags, sand patches, boost pads, and other obstacles in muted colors (warm gold, soft tan, gentle blues).
- **Overall feel**: Minimalist, soothing, almost like a watercolor mini golf course.

## Core Features

### 8 Handcrafted Holes
- **Hole 1 (Par 2)**: Gentle S-curve opener with one tee area.
- **Hole 2 (Par 3)**: Sweeping boomerang bend; sand trap inside the curve.
- **Hole 3 (Par 4)**: Hairpin turn — up, around, and back down.
- **Hole 4 (Par 3)**: Wide green with a central island; go left or right.
- **Hole 5 (Par 4)**: Long winding river with bumper and booster.
- **Hole 6 (Par 4)**: Wide fan fairway with a curved wall inside.
- **Hole 7 (Par 4)**: Horseshoe shape — cup ringed by a near-closed curved wall.
- **Hole 8 (Par 5)**: Grand tour; long meander to a ringed green with an island.

Each hole progressively teaches mechanics and builds challenge.

### Obstacles & Interactive Elements
- **Bumpers**: Spring-loaded bumps that redirect the ball.
- **Sand patches**: Slow the ball but don't stop it.
- **Boost pads**: Launch the ball in a given direction with extra speed.
- **Curved walls**: Follow the fairway's shape for natural-looking obstacles.
- **Raised islands/pillars**: The ball rolls around them; they don't block, just guide.
- **Breakable barriers**: Hit hard enough, they fall out of the way.
- **Spinners**: Rotating arms that push the ball as it passes.
- **Coins**: Collectibles scattered around holes for bonus points.

### Scoring & Progression
- Each hole has a par (target stroke count).
- Score is tracked per hole and per round.
- Best round is saved and displayed.
- Coin collection adds to a global counter.

### Full Level Editor (On-Watch)
- **Create custom courses** directly on the watch.
- **Edit elements**: drag waypoints to reshape the fairway, add/remove obstacles, place the cup.
- **Rotate and scale** obstacles with intuitive gestures.
- **Test immediately**: play your course right after designing it.
- **Save locally**: custom courses persist and appear in the course list alongside built-ins.
- **Factory reset**: revert to the original 8 holes anytime.

## User Experience

### Play Flow
1. Launch app → see the course list (built-in + custom).
2. Select a hole → see tee position and aim.
3. Drag to aim → see power preview.
4. Release → ball rolls, camera follows smoothly.
5. Hole out → see stroke count and par comparison.
6. Arrow buttons to navigate to next hole.

### Editor Flow
1. Long-press or tap "Edit" button.
2. See a palette of elements to add (waypoints, obstacles, etc.).
3. Tap an element type → tap on the course to place it.
4. Tap a placed element to select → drag to move, pinch to rotate/scale.
5. Confirm to save custom course.
6. Exit editor and play.

## Audio & Haptics

- **Slingshot release**: Crisp click haptic.
- **Ball bounces**: Bucketed by impact speed — soft click for slow bumps, stronger notifications for hard hits.
- **Obstacles**: Unique haptics for bumpers, spinners, barriers breaking.
- **Coin collection**: Light, cheerful click.
- **Hole complete**: Satisfying success haptic.
- **Ambient sounds** (optional): Gentle ball-roll ambience, soft wall impact tones.

## Target Feel

**Calm, satisfying, meditative.** The game should feel like a mental break — not frantic. Courses should encourage strategy and precision, not speed. The physics should reward good aim and planning. Every collision should feel weighty and intentional. The visuals should be soothing but clear. Editing should feel empowering and intuitive, not overwhelming.

---

This brief describes *what* the game is. Implementation details (frameworks, rendering techniques, specific services) are left to the development team.
 