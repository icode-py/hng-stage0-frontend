

# HNG Stage 1a - Advanced Todo Card

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

# HNG Stage 1B - Profile Card

A testable, accessible, responsive profile card component with real-time epoch time display.

## Live Demo

🔗 **Live URL**: [https://icode-py.github.io/hng-stage0-frontend/profile-card.html](https://icode-py.github.io/hng-stage0-frontend/profile-card.html)

## Features

- ✅ **Real-time epoch time** updates every 500ms
- ✅ **Semantic HTML** - article, figure, nav, section
- ✅ **Complete accessibility** - WCAG AA compliant
- ✅ **Fully responsive** - Mobile → Tablet → Desktop
- ✅ **Social links** open in new tabs with security attributes
- ✅ **All required data-testid attributes** for testing
- ✅ **Keyboard navigable** with focus trapping

## How to Run Locally

```bash
# Clone the repository
git clone https://github.com/icode-py/hng-stage0-frontend.git

# Open profile-card.html in your browser
open profile-card.html

## How to Run Locally


```bash
# Clone the repository
git clone https://github.com/icode-py/hng-stage0-frontend.git

# Open index.html in your browser
open index.html



## New Design Decisions for 1a
Left Border Priority Indicator - Clean visual without extra text

Inline Edit Mode - Stays on same card instead of modal

45-Second Time Updates - Balances accuracy with performance

100-Character Collapse Threshold - Optimal for readability



## Known Limitations 1a
Delete button uses confirm dialog (could be modal)

No localStorage persistence (refreshing resets state)

Due date picker limited to datetime-local format

## Built With
HTML5 (Semantic)

CSS3 (Flexbox, Grid)

Vanilla JavaScript (ES6+)

GitHub Pages

Technical Decisions for 1b
500ms Time Updates - Provides smooth real-time feel while maintaining performance

Avatar from Random User API - Uses reliable external image service

Grid Layout for Interests - Clean separation of hobbies and dislikes

Focus Trap Implementation - Enhanced keyboard navigation within card

CSS Grid + Flexbox - Modern responsive approach

Accessibility Features
Semantic HTML structure

ARIA labels and landmarks

aria-live="polite" for dynamic time updates

Visible focus indicators

Keyboard navigation with focus trap

High contrast color scheme (WCAG AA)

Alt text for avatar image

Browser Support
Browser	Version	Status
Chrome	90+	✅
Firefox	88+	✅
Safari	14+	✅
Edge	90+	✅
Validation Checklist
All data-testid attributes present

Semantic HTML used throughout

Time shows accurate milliseconds

Avatar has alt text

Social links open in new tab with security attributes

Hobbies and dislikes as separate lists

Keyboard navigation works

Responsive at 320px, 768px, 1024px+

Credits
Built for HNG Frontend Track - Stage 1B

HNG Internship

Hire Frontend Developers
