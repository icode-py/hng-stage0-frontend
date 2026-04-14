

# HNG Stage 1 - Advanced Todo Card

Interactive, stateful todo card component with edit mode, status transitions, priority changes, expand/collapse behavior, and dynamic time handling.

## Live Demo

🔗 **Live URL**: [https://icode-py.github.io/hng-stage0-frontend/](https://icode-py.github.io/hng-stage0-frontend/)

## What Changed from Stage 0

### New Features
- **Edit Mode**: Complete form to edit all task details
- **Status Control**: Dropdown to manually change status
- **Priority Visual Indicator**: Left border accent that changes color
- **Expand/Collapse**: Description collapses if too long
- **Overdue Indicator**: Visual warning when task is past due
- **Granular Time Remaining**: Shows minutes, hours, or days
- **Status Synchronization**: Checkbox and status control stay in sync

### Technical Improvements
- Added `aria-expanded` and `aria-controls` for collapse
- Added `aria-live="polite"` for time updates
- Enhanced keyboard navigation flow
- Improved responsive layout for edit form
- Added focus trapping in edit mode

## How to Run Locally

```bash
# Clone the repository
git clone https://github.com/icode-py/hng-stage0-frontend.git

# Open index.html in your browser
open index.html

## New Design Decisions
Left Border Priority Indicator - Clean visual without extra text

Inline Edit Mode - Stays on same card instead of modal

45-Second Time Updates - Balances accuracy with performance

100-Character Collapse Threshold - Optimal for readability

## Accessibility Notes
All edit form fields have proper <label for="">

Status dropdown has accessible name via aria-label

Expand toggle uses aria-expanded and aria-controls

Time updates use aria-live="polite"

Full keyboard navigation (Tab order preserved)

## Known Limitations
Delete button uses confirm dialog (could be modal)

No localStorage persistence (refreshing resets state)

Due date picker limited to datetime-local format

## Built With
HTML5 (Semantic)

CSS3 (Flexbox, Grid)

Vanilla JavaScript (ES6+)

GitHub Pages
