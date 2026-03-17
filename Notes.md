# Developer Log

---

## 2026-01-26

### session log
- Began restructuring bookmark system into a context-oriented system.
- Created two top-level bookmark folders:
  - `/transform`
  - `/database`
- Added tagging layer for granular filtering.
- Created `Template.md` and added a “Revisited” section for future updates.

### concepts
- Tech stacks age quickly; principles age well.
- Organizing by technology creates long-term clutter.
- Context > subject naming.
- Systems should scale with thinking, not just storage.

### to-do
- Finish migrating remaining bookmarks into the new structure.
- Validate whether `/transform` and `/database` truly cover ~50% of use cases.
- Reduce bookmark volume — eliminate passive collecting.

---

## 2026-01-27

### session log
- Continued portfolio development using dev server (browser-rendered).
- Continued bookmark migration process.

### concepts
- Exposure matters — building publicly increases clarity.
- Accumulation without intention creates cognitive drag.
- A clean system improves execution speed.

### to-do
- Finish bookmark overhaul completely.
- Lock portfolio structure and move from “starter excitement” to disciplined iteration.

---

## 2026-02-08

### session log
- Completed system updates and optimizations.
- Developer profile now live and updated.
- Fully switched from Windows to Ubuntu.
- Ubuntu dev workflow fully functional.
- Bookmark system officially context-driven.

### concepts
- Environment matters. Ubuntu aligns better with long-term dev goals.
- Context markers outperform subject folders.
- Systems reduce friction more than motivation does.

### to-do
- Tighten Ubuntu environment toward production parity.
- Reduce unnecessary OS friction.
- Focus on output rather than system tweaking.

---

## 2026-02-15

### session log
- Continued configuring Ubuntu dev environment.
- Worked on portfolio wireframes and defined rough content direction.
- MailWizz progressing:
  - Self-contained in single repository.
  - Separate Dockerfiles for dev and production environments.
- Continuing degree coursework at Maestro University.
- Started GenAI course via Zero To Mastery (ahead of degree timeline).

### concepts
- Waiting for curriculum pacing is optional — initiative creates advantage.
- Separating dev and prod early prevents architectural debt.
- Clear content direction reduces friction in execution.

### to-do
- Finalize Ubuntu environment stability.
- Complete MailWizz dev/prod separation cleanly.
- Establish consistent GenAI study cadence.

---

## 🛠️ 2026-02-16

### 🔹 session log
- Cleaned up bookmarks and removed stale entries  
- Expanded tagging system for better context and depth  
- Studied differences between **Vite** and **Rollup**  
  - Vite provides **dev-tools**; Rollup handles production bundling  
  - During development, Vite **does not bundle**—bundling happens only for production  

### 🔹 concepts
- Modern dev tooling favors **fast development over immediate bundling**  
- Understanding tooling philosophy helps structure workflow efficiently  
- Contextual organization and tagging improves knowledge retrieval
- Learned what a code-fence was

### 🔹 to-do
- Read and take structured notes on **Tailwind CSS** (portfolio relevance)  
- Complete **Maestro coursework**  
- Optional: watch **Zero to Mastery – LLM** lesson

  ---

## 🛠️ 2026-03-09

### 🔹 session log
- Completed a focused **1-hour deep study session** and recorded the session as a screencast for portfolio documentation  
- Began experimenting with **screen recordings as proof-of-work artifacts** to better represent study discipline and development process  
- Explored **Python fundamentals** alongside existing JavaScript knowledge  
- Discussed Python data structures and language concepts  
  - Reviewed **Python data types**  
  - Learned what **tuples** are and how they differ from lists  
  - Compared Python methods like `pop()` with JavaScript equivalents  
- Reflected on how prior **JavaScript experience makes Python feel simpler and cleaner**  
- Discussed the **evolutionary tree of programming languages** and how many modern languages borrow ideas from older paradigms  
- Began designing a **better workflow for documenting development progress** beyond simple daily dev notes  
- Evaluated file naming strategy for recorded study sessions

### 🔹 concepts
- Programming languages often evolve by **borrowing abstractions from earlier languages**  
- JavaScript can be difficult for beginners because it mixes **multiple paradigms and historical design decisions**  
- Python emphasizes **readability and simplicity**, which can feel easier after learning JavaScript  
- Recording study sessions can serve as **high-signal portfolio evidence of real work and discipline**  
- Process documentation can be as valuable as finished projects when demonstrating developer growth

### 🔹 to-do
- Continue recording **focused study sessions** for portfolio documentation  
- Develop a **consistent naming convention** for screencast recordings  
- Explore **automating session logs** from study recordings and dev activity  
- Continue progressing through **Maestro Python coursework**

---

## 2026-03-10

### session log
- Continued structured Python study session focused on data structures.
- Strengthened understanding of stacks and queues as part of Maestro.org coursework.
- Reviewed how abstract data structures map to real Python implementations.
- Completed Maestro lessons covering:
  - Stack operations (push and pop).
  - Building stacks using Python lists.
  - Applying stacks to implement undo behavior.
  - Stack challenge exercises.
  - FIFO (First In, First Out) concept.
  - Introduction to queues.
  - Queue operations (enqueue and dequeue).
  - Implementing queues using `collections.deque`.
  - Queue challenge exercises.
  - Integrating stacks and queues together conceptually.
- Practiced translating theoretical operations into Python methods:
  - `append()` as push/enqueue.
  - `pop()` as pop.
  - `popleft()` with `deque` as dequeue.
- Reinforced Python fundamentals through additional review on W3Schools.
- Compared Python data structure implementations with equivalent JavaScript concepts.
- Practiced writing safe queue operations (checking for empty structures before removing items).

### concepts
- Stacks follow LIFO (Last In, First Out).
- Core stack operations are push and pop.
- Python stacks are commonly implemented using lists.
- Queues follow FIFO (First In, First Out).
- Core queue operations are enqueue and dequeue.
- `collections.deque` is the preferred Python structure for queues because it supports efficient front removal.
- Abstract data structures describe behavior, not specific implementations.
- Python methods often serve as practical equivalents to algorithm terminology.
- Many real systems use stacks for undo history and queues for task processing.

### to-do
- Continue progressing through Maestro.org Python coursework.
- Practice implementing stacks and queues without reference material.
- Continue reinforcing Python fundamentals through W3Schools review.
- Explore real-world applications of queues such as task processing systems.
- Maintain daily session logs to document learning progress and development discipline.

---

## 2026-03-14

### session log
- Continued development work on the MailWizz project infrastructure and repository organization.
- Finalized the first dev-ready infrastructure release for the MailWizz development stack.
- Created a GitHub release capturing the stable baseline of the Docker-based development environment.
- Confirmed repository scope as **infrastructure-only**, separating environment setup from the MailWizz application source.
- Clarified that the infrastructure repo enables a developer to:
  - extract the MailWizz source
  - run the Docker build
  - launch a fully working development environment with minimal commands.
- Evaluated repository structure and removed unnecessary files to keep the project lightweight and focused.
- Moved extended documentation into the **GitHub Wiki** to reduce repository clutter and improve maintainability.
- Cleaned up README references that previously pointed to documentation files that no longer live inside the repo.
- Discussed release note wording and milestone naming for the first infrastructure release.
- Reviewed the role of scaffolding vs runtime configuration during early project development.
- Continued reinforcing Git workflow discipline around releases, documentation structure, and repository organization.

### concepts
- Infrastructure repositories should focus on environment provisioning rather than application code.
- Separating infrastructure from application source improves maintainability and scalability.
- GitHub Releases can act as stable checkpoints in project evolution.
- Documentation can live outside the repository (wiki or external docs) to keep repositories smaller and cleaner.
- Clear repository scope helps avoid mixing infrastructure, runtime artifacts, and application code.

### to-do
- Create the dedicated repository for the MailWizz application source.
- Capture the MailWizz source in a clean state **before installer modifications**.
- Begin preparing customization strategy for MailWizz branding (logo, CSS, and identity).
- Validate that the infrastructure stack can reliably support a full reinstall from scratch.
- Continue documenting development progress as portfolio proof-of-work artifacts.

---

## 2026-03-16

### session log
- Continued development work on the MailWizz infrastructure project with focus on repository discipline and runtime environment behavior.
- Investigated a failure in the MailWizz installer caused by runtime directories being ignored by Git.
- Determined that ignoring entire runtime directories prevented the installer from creating required filesystem paths after cloning the repository.
- Identified that Git does not track empty directories, which can break applications that expect runtime paths to exist.
- Designed a fix using a pattern that ignores directory contents while preserving the directory itself through `.gitkeep` files.
- Created a formal GitHub issue documenting the problem, cause, and proposed solution.
- Reviewed best practices for Git repository hygiene, particularly around runtime artifacts and installer expectations.
- Continued improving engineering documentation through session logs and structured development notes.
- Experimented with OBS screen recording to capture real development sessions as proof-of-work artifacts for portfolio documentation.
- Reflected on the importance of recording reasoning and engineering process rather than only final results.

### concepts
- Git does not track empty directories, which can break installers that expect runtime paths to exist.
- Runtime directories should exist in the repository structure but their contents should be ignored.
- Preserving directory structure while ignoring generated files is commonly solved using `.gitkeep` patterns.
- Documenting problems as GitHub issues creates traceable engineering history within a project.
- Capturing real development sessions can serve as strong portfolio evidence of engineering discipline and workflow.

### to-do
- Implement the runtime directory fix using `.gitkeep` placeholders.
- Test the MailWizz installer after the directory structure fix.
- Commit and push the fix branch to the repository.
- Close the GitHub issue once the solution is verified.
- Continue recording development sessions to build a portfolio of engineering process artifacts.

---
