# Study Companion App (Linux) – MVP Development Plan

## 🎯 Goal of This Phase
Build a functional MVP that includes:
- A character
- A study timer
- Coin reward system
- Basic character logic
- Local data persistence

---

# 🗂 Phase 1 – Planning & Architecture

## 1.1 Technical Decisions
- Choose programming language
- Choose GUI framework (GTK / Qt / etc.)
- Define project structure
- Separate UI, business logic, and data layer

## 1.2 Core Logic Decisions
- Default session length (e.g., 25 minutes?)
- Allow pause or not?
- Coin calculation logic
- Penalty for interrupting session (yes/no)

---

# 🐰 Phase 2 – Character Implementation

## 2.1 Character Design
- Create static asset (PNG or SVG)
- Minimum states:
  - `idle`
  - `happy` (after completed session)

## 2.2 Character System
- Display character in main window
- Ability to switch states programmatically
- Basic state manager module

---

# ⏱ Phase 3 – Timer Implementation

## 3.1 Timer Logic
- Set session duration
- Buttons:
  - Start
  - Pause
  - Reset
- Countdown logic
- Handle background execution correctly

## 3.2 Session Completion
- Notification when finished
- Change character state
- Trigger coin reward

---

# 💰 Phase 4 – Coin System

## 4.1 Reward Logic
Option A:
- 1 minute = 1 coin

Option B:
- Fixed reward per completed session

## 4.2 Data Persistence
- Store locally (JSON or SQLite)
- Save:
  - Total coins
  - Completed sessions count
  - Last session date

---

# 🙂 Phase 5 – Basic Character Logic

Add simple emotional system:

States:
- `happy` – after successful sessions
- `neutral` – default state
- `sad` – if session interrupted

Rules example:
- Completed session → happiness +
- Interrupted session → happiness -

---

# 🧪 Phase 6 – Testing

- Verify timer accuracy
- Test pause/resume behavior
- Confirm correct coin calculation
- Ensure data persists after app restart
- Check character state transitions

---

# 🚫 Not Included in MVP

- Statistics graphs
- Shop system
- Advanced animations
- Achievements
- Cloud sync
- Multiple characters

---

# ✅ MVP Definition of Done

- Character renders correctly
- Timer works reliably
- Coins are awarded correctly
- Data is saved locally
- Basic emotional logic functions properly

---

# ⏳ Estimated Timeline
2–3 weeks of development.
