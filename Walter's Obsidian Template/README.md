---
up:
date: 2025-08-30
updated: 2025-08-31T12:36
journal: "[[2025-08-30]]"
category:
type:
status: Active
related:
---


## Hello

My name is **Walter Strnad**. I've been using Obsidian since 2020, and I’m excited to share with you a **clean, automated note taking structure** that is both **future proof** and designed for **easy organization, journaling, and retrieval**.

I’ve spent countless hours fine-tuning this system, and I hope it saves you time and helps you stay organized. 

Feel free to reach out to me if you have any questions!
Take care, and happy note-taking! ✨

Feeling generous? [Buy me a coffee ☕️](https://ko-fi.com/hikingwithwalter) 





When you're ready, [[Home]] awaits you.

---
# General Usage Tips
1. Be careful when utilizing "New" on bases inside [[Books]], [[Watchlist]] and [[Journal Collection - 2025]]
	-  There is a current bug with Templater and periodic note plugins that don't generate templates properly or cause the properties in the notes to become unordered.

---

# Hierarchy 

### Home
- **Home**: Central dashboard for navigation, quick access, and an overview of active areas.

### Archive
- **Archive**: Storage for completed or inactive notes, kept for reference.
  - **Completed**: Finished notes stored long-term.
  - **Inactive**: Paused/abandoned notes; not actively maintained.
  - **Old**: Legacy content kept for historical context.

### Cards
- **Cards**: Atomic notes that feed MOCs, projects, and references.

### Inbox
- **Inbox**: Temporary holding area for quick captures before sorting.

### Projects
- **Projects**: Goal‑driven initiatives with outcomes and supporting notes.
  - **Active**: Current initiatives with ongoing work.
  - **Inactive**: Parked or completed initiatives kept for reference.

### Resources
- **Resources**: External materials and structured collections for study/reuse.
  - **Bookmarks**: Saved links and web resources.
  - **Documents**: Personal files/records for quick access.
  - **Locations**: Places, regions, and environments.
  - **Media**: Entertainment and study libraries.
    - **Books**: Reading list and book notes (to read/in progress/completed).
    - **Movies and TV**: Watchlist and viewing notes.
  - **People**: Profiles with roles, relationships, and context.
    - **Personal**: Personal contacts and acquaintances.
    - **Public**: Public figures and historical individuals.
  - **References**: Captured external knowledge with citations.
    - **Articles**: Online/print articles.
    - **Manuals**: Technical/user manuals.
    - **Papers**: Academic/research papers.
    - **Quotes**: Quotations with attribution.
    - **Social**: Selected social posts.
    - **Video**: Videos for study or later viewing.
  - **Obsidian**: Vault scaffolding and helpers.
    - **Attachments**: Binary assets.
      - **Images**, **PDFs**, **Videos**
    - **Banners**: Header images.
    - **Bases**: Prebuilt Base views for listing/filtering.
    - **Functions and Scripts**: Helpers (e.g., buttons/commands).
    - **Indexes**: Navigation aids (reserved).
    - **Libraries**: Hub notes aggregating MOCs by domain.
    - **Templates**: Blueprints for consistent note structure.

### Spaces
- **Spaces**: Thematic areas grouping related MOCs, projects, and resources.
  - **Knowledge**: Subject‑matter domains organized as MOCs.
    - **MOCs**: Topic maps by field.
      - **Creativity and Expression**: Gaming, Music, Photography, etc.
      - **Outdoors**: Hiking, Fishing, Fauna, Flora, etc.
      - **Science & Technology**: Astronomy, CS, Engineering, etc.
      - **Society and Systems**: History/Politics, Law, Economics, etc.
  - **Life**: Personal systems, records, and routines.
    - **Calendar**: Time‑based journaling and planning.
      - **2025**: Yearly journal and adventures.
        - **Adventures**: Entries by date - defined by `Adventure` checkbox property
        - **Daily Journal**: Dated daily notes (events, notes, photos).
        - **Journal Collection - 2025**: Cards overview of 2025 daily notes.
    - **MOCs**: Personal domains and logs.
      - **Finances**: Budgets and financial records.
      - **Health**: Wellness and routines.
      - **Household**: Home maintenance, inventories, etc. 
      - **Misc**: Other personal systems and tracking.
      - **Outdoors**: Life‑side logs/lists (adventures, summits, catches).
        - **Adventure Collection - 2025**: Year’s adventure overview.
        - **Bucket List**: Planned goals and experiences.
        - **Fishing Log**: Catches, locations, conditions.
        - **Summit Log**: Peaks with dates/routes/notes.
  - **Work**: Workspace for professional projects and notes (reserved).

-----

# Properties

up:
- Parent note link used for navigation and hierarchy.

date:
- Creation or event date; used for sorting and journal queries.

updated:
- Last modified timestamp; shown in lists/tables. (automatically synced via plugin: "Update Time on Edit")

type:
- Note kind (e.g., Library, MOC, Daily Journal, Project, Reference, Media, Document).

status:
- Lifecycle/state (e.g., Active, Inactive, Reading, Later, Completed, Watching).

category:
- High-level area (e.g., Life, Knowledge, Project, Resource, Media).

journal:
- Link to the related daily note.

related:
- Links to associated notes/entities.

desc:
- Short description shown in table views/cards.

---

# Core plugins
- **Backlinks**: Shows all notes that link to the current note.
- **Command palette**: Quick access to any Obsidian command via search.
- **File recovery**: Restores previous versions of notes in case of accidental edits or deletion.
- **Page preview**: Hover over a link to preview its content without opening the note.
- **Sync**: Syncs notes, settings, and attachments across devices using Obsidian Sync.

# Community plugins
- **BRAT**: Install and test beta plugins directly from GitHub repositories.
	- Used for beta release of Templater.
- **Callout Manager**: Customize and create callout styles for better note formatting.
- **Dataview**: Query and display note data dynamically using properties and metadata.
	- Used for "Unrequited links"
- **Iconize**: Add icons to notes, links, and properties for visual organization.
- **Note Toolbar**: Adds customizable toolbar buttons for quick actions in the editor.
	- Used for "Previous - Today - Next" in Daily Journal navigation
- **Periodic Notes**: Automates creation of daily, weekly, and monthly notes with templates.
- **Pixel Banner**: Display custom banners at the top of notes for style or context.
- **Templater**: Insert and execute templates with variables, scripts, and dynamic data.
- **Update time on edit**: Automatically updates a property (e.g., `updated`) when a note is modified.