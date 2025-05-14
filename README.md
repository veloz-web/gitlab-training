Training Plan Modules:

Module 1: Introduction & GitLab Basics (30-60 mins)

Objective: Understand the context of GitLab's project management tools and navigate the basic UI.
Topics:
What is GitLab? (Brief overview: Source Code Management + CI/CD + Project Management).
Focus: The "Plan" stage capabilities.
GitLab UI Tour: Dashboard, Groups, Projects, Key sidebar menus (Issues, Boards, Epics, Milestones).
Groups vs. Projects: How work is organized.
Creating/Navigating a Project: Setting up a space for practice.
Activities:
Log in to GitLab.
Navigate the main dashboard.
Create a new Project (or use a pre-created sandbox project).
Explore the project's sidebar menus.
Module 2: Issues - The Core Work Item (60-90 mins)

Objective: Learn how to create, manage, and understand individual work items (tasks, user stories, bugs).
Topics:
What is a GitLab Issue? (The fundamental unit of trackable work).
Creating Issues: Title, Description (Markdown formatting), Assignees, Due Dates.
Issue Details: Comments, Activity log, Notifications, Linking related items.
Issue Types (if configured/available): Differentiating between bugs, features, tasks, etc.
Managing Issues: Editing, Closing, Reopening, Locking conversations.
Issue List View: Sorting, Filtering (by assignee, author, label, milestone, etc.).
Quick Actions: Using commands in comments/descriptions for efficiency (e.g., /assign, /label, /milestone).
Activities:
Create several sample issues representing backlog items (e.g., "Implement user login," "Fix button alignment," "Write API documentation").
Assign issues to yourself or team members (if applicable).
Add comments and use Markdown formatting.
Practice filtering the issue list.
Use a quick action to assign or add a label (preview for next module).
Module 3: Labels - Categorization & Status Tracking (45-75 mins)

Objective: Use labels to categorize issues and, crucially, track their status (backlog status).
Topics:
What are Labels? (Keywords for organization).
Project vs. Group Labels: Scope and inheritance.
Creating Labels: Naming conventions, color coding.
Scoped Labels: The key to managing exclusive states (e.g., Status::, Priority::, Type::).
Tracking Backlog Status: Defining and creating status labels (e.g., Status::Backlog, Status::ToDo, Status::InProgress, Status::Review, Status::Done).
Applying Labels: Adding/removing labels from issues.
Filtering by Labels: Finding all "High Priority" bugs or all "InProgress" items.
Activities:
Navigate to the Labels section (Project or Group level).
Create a set of scoped status labels (Status::Backlog, Status::ToDo, etc.).
Create other useful labels (e.g., Type::Bug, Type::Feature, Priority::High).
Apply various labels (including status labels) to the previously created issues.
Practice filtering the issue list by different labels, especially status.
Module 4: Milestones - Timeboxing & Release Planning (45-60 mins)

Objective: Group issues into time-bound periods (sprints, iterations, releases).
Topics:
What are Milestones? (Representing sprints, releases, or phases with start/end dates).
Creating Milestones: Title, Start Date, Due Date, Description.
Assigning Issues to Milestones: Linking work to specific timeboxes.
Milestone View: Progress tracking (burndown charts - Note: availability varies by tier), list of associated issues, linked merge requests.
Using Milestones for Sprints vs. Releases.
Filtering Issues by Milestone.
Activities:
Create two Milestones (e.g., "Sprint 1 - April", "Q2 Release").
Assign some issues to "Sprint 1 - April".
Assign other issues (perhaps including one representing a larger deliverable) to "Q2 Release".
Explore the Milestone view page for "Sprint 1 - April".
Filter the issue list to show only items in "Sprint 1 - April".
Module 5: Epics - Grouping Large Initiatives (45-75 mins) - Note: Premium/Ultimate Feature

Objective: Organize related issues and potentially other epics under larger themes or features.
Topics:
What are Epics? (Containers for strategic initiatives spanning multiple issues/milestones).
Note: Clearly state this is often a paid feature (GitLab Premium/Ultimate). If using Free tier, explain the concept but skip hands-on or discuss workarounds (e.g., using specific labels).
Creating Epics: Title, Description, Start/End Dates (fixed or inherited).
Epic Hierarchy: Adding child epics and child issues.
Viewing Epics: Tree structure, Roadmap view.
Epics vs. Milestones: Purpose and usage differences (Theme/Initiative vs. Timebox).
Activities (If feature available):
Navigate to the Epics section (usually at the Group level).
Create an Epic (e.g., "User Management Revamp").
Add existing issues (like "Implement user login") as children to the Epic.
Create another, smaller Epic (e.g., "Profile Page Enhancements") and add it as a child to the main Epic.
Explore the Epic tree view.
Module 6: Issue Boards - Visualizing Workflow (60-90 mins)

Objective: Create and use Kanban-style boards to visualize and manage the flow of work based on status labels or other criteria.
Topics:
What are Issue Boards? (Visual workflow tool).
Default Boards: How they are initially configured.
Creating Custom Boards: Defining the scope (entire project, specific milestone, etc.).
Configuring Board Columns:
List Settings: Adding columns based on Labels (most common for status), Assignees, or Milestones.
Mapping Status: Setting up columns corresponding to your Status:: labels (ToDo, InProgress, Done).
Using the Board: Dragging and dropping issues between columns to update their status (label).
Board Filtering: Focusing the board view.
Multiple Boards: Creating boards for different teams, workflows, or views.
Activities:
Navigate to Issue Boards.
Explore the default board.
Create a new board named "Development Workflow".
Configure columns based on the Status:: labels created earlier (Backlog, ToDo, InProgress, Review, Done).
Drag and drop issues between columns; verify the labels update on the issues themselves.
Create another board focused only on issues within the "Sprint 1 - April" milestone.


Module 7: Roadmaps & Other Planning Tools (30-60 mins) - Note: Partially Premium/Ultimate

Objective: Understand higher-level timeline visualization and other relevant planning features.
Topics:
Roadmap View (Note: Premium/Ultimate Feature): Visualizing Epics over time based on their start/end dates. Gantt-like overview.
Iteration Cadences (Note: Often Premium/Ultimate): An alternative/complement to Milestones for managing automated sprint schedules. Briefly explain if relevant/available.
Analytics (Value Stream, Burndown/Burnup Charts): Overview of reporting capabilities (Note: Availability varies significantly by tier).
Activities (If features available):
Explore the Roadmap view (if Epics are used).
Briefly look at any available Analytics charts related to issues/milestones.
Module 8: Tying it Together & Best Practices (30 mins)

Objective: Recap the workflow and discuss tips for effective use.
Topics:
Review: Typical workflow (Idea -> Epic -> Issue -> Backlog Label -> Milestone Planning -> Board Movement -> Done).
Consistency is Key: Importance of standardized labels and milestone usage.
Using Issue Templates: Speeding up issue creation for common types (bugs, features).
Notifications: Managing your GitLab updates.
Linking Issues, Merge Requests, and Commits: Connecting code changes back to requirements/tasks.
Activities:
Discussion: Q&A, how to apply this to the team's specific context.
Review a sample issue showing links to MRs or other issues.
