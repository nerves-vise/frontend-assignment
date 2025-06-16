# 🧪 Frontend Assignment – Team Member Dashboard

## 🧠 Objective

Build a dashboard-style web application for managing team members in an organization.  
This assignment evaluates your skills in state management, dynamic UI, component structure, and edge case handling.

Use any modern frontend stack. Backend is **not required** — all state is local.

---

## 📂 Features to Implement

### 1. 🧍 Team Member List
- Display a list of team members
- Show: name, email, role, team, status (active/inactive)
- Filter by role, team, and status
- Search by name/email
- Remove a member (with confirmation modal)

### 2. ➕ Add/Edit Member Form
- Modal for adding or editing a member
- Validate inputs (required fields, email format)
- Status toggle (active/inactive)

### 3. ✉️ **Pending Invitations** (⚠️ Special behavior)
- Simulate a list of pending invites (name, email, role, team)
- Each invite auto-expires after **30 seconds**
- Show countdown timer per invite
- Buttons:
  - ✅ Approve → moves to team list
  - ❌ Cancel → removes immediately
- If not handled in time → auto-delete with toast/notice

> This is intentionally tricky to test how you handle timers, state sync, and cleanup logic.

---

## 🧰 Tech Stack

You may use:
- React (with Vite, CRA, or Next.js)
- Any UI framework (Tailwind, Chakra, MUI, or custom)
- State via `useState`, `useReducer`, Context, Zustand, etc.
- No backend: store everything in memory or `localStorage` (optional)

---

## 📦 Sample Data Format

```js
const members = [
  {
    id: 1,
    name: "Alice",
    email: "alice@company.com",
    role: "Designer",
    team: "UX",
    status: "active"
  }
];

const pendingInvites = [
  {
    id: 101,
    name: "Bob",
    email: "bob@company.com",
    role: "Engineer",
    team: "Dev",
    expiresIn: 30 // seconds
  }
];

## ✅ Bonus Features (Optional)

- Persist data to localStorage
- Responsive layout
- Search with fuzzy matching (e.g. Fuse.js)
- Unit testing (Jest + RTL)
- Animations or transitions
- Sorting by name or team

## 🧪 Evaluation Criteria

| Area             | Details                                 |
| ---------------- | --------------------------------------- |
| Functionality    | Core features complete and usable       |
| Component design | Reusable and well-structured components |
| State handling   | Clear separation and updates            |
| UI/UX            | Intuitive, responsive, consistent       |
| Code quality     | Clean, maintainable, and modular        |
| Bonus            | Persistence, testing, extra UX polish   |


## 🚀 Submission

- Push to a public Git repository
- Include a README.md with:
  - Setup instructions
  - Any assumptions or notes
- Submit the link once ready



## 🎉 Good luck — looking forward to seeing your approach!




