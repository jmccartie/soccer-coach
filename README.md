# Soccer Coach

A single-page web app for managing a youth soccer lineup on the sideline. Drag players between the bench, field positions, and the subbed-out list. State is saved automatically to `localStorage`.

## Usage

Open [index.html](index.html) in a browser. No build step, no server.

### Roster

- Type names into the input and press **Add** (or Enter). Comma-separated names are accepted.
- **Shuffle Roster** randomizes bench order.
- **Edit** reveals a × on each player to remove them.

### Lineup

- Drag players from the bench onto any field slot (forwards, mids, backs, goalie).
- Dropping a player on an occupied slot swaps the current occupant back to the source.
- Drag a player from a field slot to **Subbed Out** to increment their sub count (shown as a red badge).
- Tap the red sub badge to reset that player's count to 0.

### Buttons

- **Edit** — toggle remove-mode on players.
- **Reset Positions** — move every player back to the bench and clear all sub counts.
- **New Game** — clear all players and state.

## Storage

Everything persists in `localStorage` under the key `soccer-coach-state-v1`. Clearing site data resets the app.

## Dependencies

- [SortableJS](https://sortablejs.github.io/Sortable/) via CDN for drag-and-drop.

## Coaching Staff

Built with [Claude Code](https://claude.com/claude-code) — an assistant coach who never asks for orange slices.
