# HNG Stage 0 - Todo Task Card

A fully accessible, responsive todo task card component built for the HNG Frontend Track Stage 0 task. This component features real-time time remaining updates, semantic HTML, complete keyboard navigation, and all required test IDs for automated testing.


## Live Demo

🔗 **Live URL**: [https://icode-py.github.io/hng-stage0-frontend/](https://icode-py.github.io/hng-stage0-frontend/)

## Features

- ✅ **Real-time time remaining** updates every 45 seconds
- ✅ **Complete accessibility** - WCAG AA compliant, keyboard navigable
- ✅ **Fully responsive** - Works perfectly from 320px to 1200px+
- ✅ **Semantic HTML** - article, time, lists, proper button elements
- ✅ **All test IDs included** - Ready for automated testing
- ✅ **Interactive completion toggle** - Checkbox with visual feedback
- ✅ **Priority badges** with color coding (High/Medium/Low)
- ✅ **Tag system** with customizable categories

## Technologies Used

- HTML5 (Semantic)
- CSS3 (Flexbox, Grid, Media Queries)
- Vanilla JavaScript (ES6+)
- GitHub Pages (Hosting)

## How to Run Locally

### Option 1: Direct Download
1. **Download the HTML file**
   ```bash
   curl -O https://icode-py.github.io/hng-stage0-frontend/

## Trade-offs & Limitations
No Build Step

Trade-off: No module bundling or minification

Why: Simpler for review and testing requirements

Impact: Slightly larger file size but still under 15KB

Client-Side Only

Trade-off: No persistent storage or backend

Why: Task only required frontend component

Impact: Refresh resets completion state 

Fixed Priority Value

Trade-off: Hard-coded "High" priority instead of dynamic

Why: Meets requirement while keeping scope manageable

Impact: Users can't change priority without code edit

Simple Alert Dialogs

Trade-off: Using native alert() and confirm() for edit/delete

Why: No extra dependencies, fully accessible

Impact: Less polished than modal dialogs but functional

Single Task Card

Trade-off: One card instead of multiple tasks

Why: Focused on component quality per requirements

Impact: Not a full todo app but demonstrates all features

Testing
Automated Testing Support
All required data-testid attributes are present:

test-todo-card - Card container

test-todo-title - Task title

test-todo-description - Task description

test-todo-priority - Priority badge

test-todo-due-date - Due date display

test-todo-time-remaining - Time remaining

test-todo-status - Status indicator

test-todo-complete-toggle - Checkbox

test-todo-tags - Categories list

test-todo-edit-button - Edit button

test-todo-delete-button - Delete button

Manual Testing Checklist
Tab navigation reaches: Checkbox → Edit → Delete buttons

Space/Enter toggles checkbox

Time remaining updates within 60 seconds

Card stacks vertically on mobile

No horizontal scroll at any width

Screen reader announces all content