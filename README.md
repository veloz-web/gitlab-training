Revised Training Plan Modules:

Module 1: Optimizing Your GitLab Environment & Workflow (30-45 mins)

Objective: Fine-tune the GitLab environment and individual settings for power users.
Topics:
Advanced Notification Settings: Custom levels, Todos, Email filters.
Profile Settings & Preferences: SSH Keys, GPG Keys, Theme, Syntax Highlighting.
Project & Group Settings Deep Dive: Key configurations often overlooked (e.g., default branch protection, merge request settings, wiki/snippet visibility).
Understanding GitLab Tiers: Briefly touch on how Free/Premium/Ultimate affects feature availability for topics covered.
Activities:
Review and customize personal notification settings.
Explore project settings relevant to upcoming modules (MR defaults, CI/CD settings).
Module 2: Advanced Issue Management & Integrated Time Tracking (75-105 mins) (Focus: Moving beyond creation to sophisticated management and data extraction)

Objective: Master advanced issue features for granular tracking, relationships, and utilize GitLab's time management capabilities.
Topics:
Issue Deep Dive:
Tasks Lists (Checklists) within Issues: Using them as lightweight sub-tasks, tracking completion.
Issue Relationships: Linked, Related, Blocking, and Blocked by issues. Visualizing dependencies.
Promoting Issues to Epics.
Moving Issues between projects.
Confidential Issues & Locking Issues.
Issue Health Status (At-Risk, Needs Attention, On Track - Premium/Ultimate).
Service Desk: Creating issues from emails for external feedback loops.
Issue Templates: Standardizing bug reports, feature requests at project and group levels.
Time Management in GitLab:
Estimating Time: Using /estimate quick action.
Tracking Spent Time: Using /spend quick action.
Viewing Time Tracking Reports: Project-level summaries and per-issue breakdowns.
Integrating time tracking with Milestones and billing cycles (conceptual).
Limitations and best practices for accurate time logging.
Activities:
Create issues with task lists and mark items as complete.
Establish blocking relationships between two issues.
Set up a basic issue template.
Practice using /estimate and /spend on several issues.
Review the time tracking report for the project.
Discuss team conventions for time tracking.
Module 3: Strategic Labeling & Advanced Filtering Techniques (60-90 mins) (Focus: Using labels for automation triggers, complex state management, and powerful reporting)

Objective: Implement advanced labeling strategies for workflow automation, multi-faceted categorization, and precise data retrieval.
Topics:
Scoped Labels Mastery:
Designing effective scoped label systems (e.g., Workflow::, Priority::, Team::, QA::Status).
Enforcing workflow progression using scoped labels on Issue Boards.
Group Labels vs. Project Labels: Strategic decisions for consistency vs. specificity. Promoting project labels to group labels.
Labels for Automation:
Using labels to trigger CI/CD jobs (e.g., a deploy::staging label).
Conceptual: Labels as triggers for webhooks or external integrations via API.
Advanced Filtering & Searching:
Leveraging GitLab's powerful search syntax (AND/OR, exclusion, filtering by ID, reaction emojis).
Saving complex search queries for quick access.
Label Subscriptions & Notifications.
Best practices for label hygiene: Archiving, avoiding clutter, establishing naming conventions.
Activities:
Design a set of scoped labels for a hypothetical complex workflow (e.g., feature development with design, dev, QA, UAT stages).
Apply these to issues and configure an Issue Board reflecting this workflow.
Construct complex search queries using multiple labels, assignees, and other attributes.
Discuss how labels could initiate automated actions in their context.
Module 4: Work Hierarchies: Epics vs. Milestones vs. Issues/Tasks (60-75 mins)

Objective: Clearly differentiate and strategically utilize Epics, Milestones, and Issues (including task lists) for effective short-term and long-term planning.
Topics:
Epics (Strategic Themes - Primarily Premium/Ultimate):
Purpose: Grouping issues and child-epics under large initiatives or features.
Characteristics: Start/end dates (fixed or inherited), multi-level hierarchy.
Use Cases: Product roadmapping, tracking major deliverables, cross-project initiatives.
Issues (Work Items/Tasks):
Purpose: The fundamental unit of work (story, bug, task).
Task Lists within Issues (Sub-tasks): For breaking down an issue into smaller, manageable steps without creating separate formal issues. When to use this vs. separate issues.
Milestones (Time-Boxes):
Purpose: Grouping issues (and indirectly, parts of epics) into time-bound periods.
Characteristics: Start/end dates, focused on delivery cadence.
Use Cases: Sprints, iterations, release versions, phases.
Key Distinctions & Relationships:
Epic = What (the initiative), Milestone = When (the timebox), Issue = How (the specific work).
How they interact: An Epic can span multiple Milestones; a Milestone can contain Issues from multiple Epics.
Visualizing: Epics on Roadmaps, Issues in Milestones & Boards.
Activities:
Scenario-based discussion: Given a large project, map out potential Epics, child Issues, and how Milestones would apply.
Analyze how task lists within an issue could be used vs. creating separate child issues for an Epic.
If Epics are available: Create a multi-level epic structure and assign issues. View on a roadmap.
Module 5: Advanced Git Branching Workflows: Rebase vs. Merge with GitLab (60-90 mins)

Objective: Understand the implications of rebasing versus merging in Git, and how to apply these strategies effectively within a GitLab Merge Request workflow.
Topics:
Core Concepts Review:
What is git merge? (Preserves history, creates merge commits).
What is git rebase? (Rewrites history, creates a linear history).
Pros and Cons:
Merge: Traceability, explicit integration points vs. cluttered history.
Rebase: Cleaner, linear history vs. risk of rewriting shared history, potential for more complex conflict resolution (if done late).
Strategic Application:
When to Rebase: Typically on local feature branches before pushing or to update a feature branch with changes from the target branch (e.g., main).
When to Merge: Integrating main into a long-lived feature branch (to avoid constant rebasing), or as the final step of integrating a feature branch via a Merge Request if that's the chosen project strategy.
GitLab Merge Request (MR) Settings & Strategies:
Merge Commit (default).
Merge commit with semi-linear history (encourages rebase before merge).
Fast-forward merge (only if feature branch is directly ahead of target).
Squash and merge (combines all feature branch commits into one on the target branch).
Team workflows: Feature branching, Gitflow (and how rebase/merge fit).
Interactive Rebase (git rebase -i): Squashing, rewording, reordering commits on a feature branch before creating an MR or pushing for review.
Handling Merge Conflicts during Rebase vs. Merge.
Caution: Never rebase a branch that others are using and pulling from.
Activities:
Live demo/walkthrough:
Rebasing a feature branch onto main.
Merging main into a feature branch.
Resolving a simple conflict in both scenarios.
Review GitLab project settings for MRs and discuss implications of different merge methods.
Team discussion on establishing a consistent branching and merging strategy.
Module 6: Advanced Issue Board Configurations & Automation (45-60 mins)

Objective: Leverage advanced Issue Board features for highly customized workflow visualization and automation.
Topics:
Multi-list configurations: Columns based on Assignees, Milestones, Iterations (Premium/Ultimate), Labels.
WIP (Work In Progress) Limits: Setting constraints on columns.
Board Scope: Project, Group, specific Milestones, Iterations.
Swimlanes: Grouping issues horizontally by Epic (Premium/Ultimate) on a board.
Using boards for specific use cases: Bug Triage, Sprint Planning, Release Management.
Quick board actions: Creating issues directly in columns.
Activities:
Configure a board with WIP limits.
If available, set up swimlanes by Epic on a board.
Design a board specifically for a "Sprint Retrospective" or "Bug Triage" process.
Module 7: GitLab CI/CD Foundations (Refresher/Intro for Context) (30-45 mins)


Objective: Ensure a common understanding of GitLab CI/CD core components before diving into best practices.
Topics:
.gitlab-ci.yml: The heart of GitLab CI/CD.
Pipelines, Stages, Jobs: Basic structure.
Runners: Shared, Group, Specific – how they execute jobs.
Variables: Predefined, Custom, Protected, Masked.
Artifacts & Caching: Storing results and speeding up pipelines.
Activities:
Review a simple .gitlab-ci.yml file.
Identify stages, jobs, and basic keywords.
Briefly check runner availability in the project/group.
Module 8: CI/CD Pipeline Best Practices & Dynamic Test Execution (90-120 mins)

Objective: Implement CI/CD best practices for efficiency, maintainability, and security, including how to structure tests to run conditionally.
Topics:
CI/CD Best Practices:
Optimize for Speed: Small, fast jobs; parallelization (parallel: keyword); efficient Docker image usage.
Effective Caching: Dependencies, build outputs.
Secure Secrets Management: Using CI/CD variables (protected, masked), integration with HashiCorp Vault (Premium/Ultimate).
DRY Pipelines: include: for templates/common configurations, YAML anchors/aliases (&, *, <<).
Idempotent Jobs: Ensuring jobs can be re-run without negative side effects.
Review Apps: Dynamically creating environments for MRs.
Managing Pipeline Costs/Resources (especially with shared runners).
Structuring Pipeline Tests to Run "As Needs" Basis:
rules: Keyword: The modern and most flexible way.
rules:if: with CI/CD variables (predefined or custom).
rules:changes: Run jobs only if specific files/paths change (e.g., run backend tests if backend code changes).
rules:exists: Run jobs if specific files exist.
rules:when: manual for optional jobs (e.g., deployment to production).
rules:allow_failure: for non-critical jobs.
only/except (legacy but still encountered): Basic conditional execution based on branches, tags, variables, changes.
Using Variables to Control Job Execution: Setting variables in one job to be used in rules:if: of subsequent jobs.
Parent-Child Pipelines & Dynamic Pipelines: For complex scenarios where pipeline structure is determined at runtime.
Activities:
Analyze an existing .gitlab-ci.yml (or a provided example) for areas of improvement based on best practices.
Modify a CI job to run only when files in a specific directory (/backend) are changed using rules:changes:.
Create a manual job for deployment using rules:when: manual.
Discuss strategies for running different test suites (unit, integration, E2E) based on triggers (e.g., MR vs. main branch, specific code changes).
Module 9: Strategic Roadmapping & High-Level Planning (45-60 mins) - Primarily Premium/Ultimate

Objective: Utilize GitLab Roadmaps for long-term strategic visualization and communication.
Topics:
Roadmap View: Visualizing Epics over time, based on start/end dates.
Filtering and customizing the Roadmap view.
Tracking Epic progress and dependencies on the Roadmap.
Communicating strategic plans to stakeholders using Roadmaps.
Alternative for Free Tier: Discuss how labels and milestones combined can offer a simpler form of roadmap/release planning.
Activities:
If using Epics: Review the Roadmap, adjust Epic dates, and observe changes.
Discuss how this view aids in long-term planning and stakeholder communication.
Module 10: Advanced Ecosystem Integration & Automation (30-45 mins)

Objective: Briefly explore advanced automation and integration possibilities beyond the core UI.
Topics:
GitLab API: Overview of capabilities for custom automation and integration.
Webhooks: Triggering external actions based on GitLab events.
GitLab Triage (Bot): Automating common issue/MR management tasks.
Integrations: Connecting with Slack, Jira, etc. (focus on less common or more powerful integrations).
Activities:
Show examples of API usage (e.g., via curl or a simple script).
Review available project integrations.
Discuss potential automation opportunities relevant to the team.

Wrap-up & Next Steps:
Q&A tailored to advanced scenarios.
Challenge participants to identify 1-2 advanced features or practices to implement in their projects.
Resources for continued advanced learning: GitLab documentation (DevOps practices, API docs), GitLab blog for new features.
