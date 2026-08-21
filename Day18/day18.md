# Day 18 — Brain Dump Action Planner 🧠📋

## Overview

Created and tested a custom Claude Skill named **`brain-dump-action-planner`**.

The skill transforms messy notes, meeting transcripts, voice memos, brainstorming sessions, class notes, and project discussions into structured, actionable information without inventing or assuming missing details.

## Custom Skill

**Skill Name:** `brain-dump-action-planner`

**Description:**

Transform messy notes, meeting transcripts, voice memos, brainstorming sessions, and stream-of-consciousness thoughts into structured summaries, action plans, decisions, open questions, and task lists. Organize information clearly without inventing, assuming, or filling gaps. Preserve all names, dates, numbers, and terminology exactly as provided.

## Key Features

- Structured **Summary**
- **Key Takeaways** displayed as dashboard cards
- Interactive **Action Items** table
- **Owner, Deadline, and Status** tracking
- **Open Questions**
- **Risks / Blockers**
- **Conflicts**
- **Additional Notes**
- Source information for **Merge Mode**
- Speaker-based analysis in **Transcript Mode**
- Duplicate-item detection in **Merge Mode**
- Conflict Resolution Review
- Missing information shown as **"Not specified"**
- No invented, assumed, predicted, or estimated information

## Status Badges

The dashboard uses clear visual status indicators:

- 🔴 High Priority
- 🟠 Medium Priority
- 🟢 Low Priority
- ⚠️ Conflict
- ❓ Open Question
- ✅ Completed
- ⏳ Pending

## Output Modes

### Full Breakdown

Converts a complete brain dump or set of notes into a structured interactive HTML dashboard.

### Transcript Mode

Organizes transcripts using:

- Speaker Summary
- Decisions by Speaker
- Action Items by Speaker
- Attribution Notes

Speaker labels are preserved exactly as provided.

### Merge Mode

Combines information from multiple sources while preserving source context.

Includes:

- Duplicate Items
- Conflict Resolution Review
- Source Note

Conflicts are never automatically resolved.

## Dashboard Design

The generated HTML dashboard follows a modern project-management style inspired by:

- Notion
- ClickUp
- Linear
- Asana
- Airtable

It includes:

- Responsive layout
- Cards
- Tables
- Status badges
- Section headers
- Visual indicators
- Hover effects
- Soft shadows
- Collapsible sections
- Mobile responsiveness
- Clean typography
- Strong visual hierarchy

## Testing

The skill can be reused with different types of unstructured information, including:

1. Meeting Notes
2. Brainstorming Notes
3. Class Notes
4. Voice Memo Transcripts
5. Project Discussions

The same instructions do not need to be entered again each time because the logic is stored inside the custom skill.

## Key Learning

This task demonstrated how a custom AI skill can turn unstructured information into a consistent workflow.

Instead of manually reading long notes and creating task lists, the skill organizes information into:

**Notes → Summary → Key Takeaways → Action Items → Questions → Risks → Conflicts → Dashboard**

The most important principle is that the skill preserves the source information and does not fill gaps with assumptions.

## Screenshots

Add screenshots of the following:

- Custom Skill creation
- Skill name and description
- Skill instructions
- Generated interactive dashboard
- Action Items section
- Risks / Blockers section
- Open Questions section
- Testing with different note formats

