# Project Manifest

<!--
Add this file to any project folder with 10+ files.
It tells Claude which documents are the source of truth, which are secondary,
and which to ignore — preventing confused output from outdated or irrelevant files.

The underscore prefix keeps it sorted to the top of the folder.
-->

## Tier 1 — Canonical (always read first)
<!-- Source-of-truth documents. Claude must read these before starting any task. -->
<!-- Examples: current strategy doc, project brief, brand guidelines, approved pricing -->
-
-
-

## Tier 2 — Domain (load when relevant)
<!-- Subfolders or files Claude should only read when the task touches that area. -->
<!-- Format: /subfolder-name → description of what's in it -->
-
-
-

## Tier 3 — Archival (ignore unless asked)
<!-- Old drafts, superseded versions, reference material. Claude skips these by default. -->
-
-
-

## Notes
<!-- Any project-specific rules or context Claude should know -->
<!-- Examples: "Client uses 'members' not 'users'", "All deliverables in .docx format" -->

