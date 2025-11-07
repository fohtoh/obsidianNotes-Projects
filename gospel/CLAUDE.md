# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a personal gospel study vault designed for use with Obsidian. It contains the complete standard works of The Church of Jesus Christ of Latter-day Saints, including:
- Book of Mormon
- Doctrine and Covenants
- Pearl of Great Price
- Old Testament and New Testament (King James Version)
- Joseph Smith Translation (JST) of the Bible with all changes (completed before July 1833)

The vault also includes personal study materials organized by topics, scriptures, and the Come Follow Me curriculum.

## Architecture

### Directory Structure

**`scriptures/`** - Contains the full text of all standard works
- Organized by book, with folders numbered sequentially (e.g., `01 1 Nephi`, `02 2 Nephi`)
- Sequential numbering enables reading in order using file navigation
- Files are named lowercase with chapter numbers for fast linking (e.g., `1nephi01.md`, `dc001.md`)
- Each verse is formatted as a level 2 heading (`## 1.`, `## 2.`, etc.)

**`gospelStudy/`** - Personal study materials
- `scriptures/` - Christ-centered analyses and notes on specific scriptures, organized by book/chapter (e.g., `Genesis/genesis01.md`, `Moses/moses01.md`, `Abraham/abraham03.md`)
- `topics/` - Notes on gospel topics
- `comeFollowMe/` - Materials for Come Follow Me curriculum, organized by year (e.g., `2026 - Old Testament/`)

**`.obsidian/`** - Obsidian vault configuration (should not be modified manually in most cases)

### Linking System

This vault leverages Obsidian's Wikilink syntax for cross-referencing:

- **Single verse**: `[[1nephi03#7]]` links to verse 7 of 1 Nephi chapter 3
- **Multiple verses**: `[[1nephi03]]:7-9` references verses 7-9 (note in text, not a direct link)
- Each verse has an H2 heading to enable direct linking via anchors

### Content Formatting Conventions

**Scripture files**:
- Each verse is a standalone H2 heading with the verse number (`## 1.`)
- Verse text follows immediately after the heading
- No blank lines between verses

**Adding personal notes**:
- Use bullets (`-`) or blockquotes (`>`) directly after verses
- Notes specific to one verse should go right after that verse
- Principles applicable to multiple scriptures should be written as separate notes and linked

## Common Tasks

### Adding Study Notes

When adding notes to scripture files:
1. Use the Read tool to view the scripture file
2. Use the Edit tool to add notes after specific verses using bullets or blockquotes
3. For cross-cutting principles, create a new note in `gospelStudy/topics/` and link to it

### Creating Come Follow Me Materials

Materials are organized in `gospelStudy/comeFollowMe/{year}/` where year corresponds to the curriculum year (e.g., `2026 - Old Testament`).

**Come Follow Me Schedule (2026 - Old Testament):**
- Week 1 (Dec 29-Jan 4): Introduction to the Old Testament
- Week 2 (Jan 5-11): Moses 1; Abraham 3
- Week 3 (Jan 12-18): Genesis 1-2; Moses 2-3; Abraham 4-5
- Week 4 (Jan 19-25): Genesis 3-4; Moses 4-5
- Week 5 (Jan 26-Feb 1): Genesis 5; Moses 6
- Week 6 (Feb 2-8): Moses 7

### Creating Christ-Centered Analyses

This repository includes a custom **christ-centered-scholar agent** that analyzes scriptures to identify references to Jesus Christ, including both direct mentions and symbolic/typological references.

**When to use the christ-centered-scholar agent:**
- Analyzing scripture chapters for Come Follow Me preparation
- Identifying how specific passages testify of Christ
- Creating study materials that focus on the Savior

**How to use it:**
```
Use the Task tool with subagent_type="christ-centered-scholar" and provide:
- The scripture reference to analyze
- The file path to the scripture
- Context (e.g., which Come Follow Me week)
- Request for both direct and symbolic references to Christ
```

**Output location:**
Save the resulting Christ-centered analyses in `gospelStudy/scriptures/{Book}/{chapter}.md` (e.g., `gospelStudy/scriptures/Genesis/genesis01.md`, `gospelStudy/scriptures/Moses/moses01.md`)

**File naming convention:**
- Directory: Book name (e.g., `Genesis`, `Moses`, `Abraham`)
- File: Lowercase book + chapter number (e.g., `genesis01.md`, `moses01.md`, `abraham03.md`)

### Batch Renaming or Formatting

- For verse heading changes or bulk content updates: Use Edit or Write tools with regex patterns if needed
- For filename changes: Manually update or use Obsidian's "Bulk Rename" plugin (not in scope for Claude Code)

## Existing Christ-Centered Analyses

The following Christ-centered analyses have been created for Come Follow Me 2026:

**Week 2 (January 5-11):**
- `gospelStudy/scriptures/Moses/moses01.md` - Moses 1 analysis
- `gospelStudy/scriptures/Abraham/abraham03.md` - Abraham 3 analysis

**Week 3 (January 12-18):**
- `gospelStudy/scriptures/Genesis/genesis01.md` - Genesis 1 analysis

These files contain comprehensive analyses of how each scripture chapter testifies of Jesus Christ, including direct references, symbolic connections, doctrinal insights, and teaching applications.

## Important Constraints

- **Never modify scripture text** in the `scriptures/` directory unless explicitly fixing formatting issues
- **Preserve the heading structure** - Each verse must remain an H2 heading for linking to work
- **Use lowercase filenames** for all scripture files to maintain consistency
- **Do not add blank lines** between verses in scripture files
- When working with file paths containing spaces (e.g., "2026 - Old Testament"), always quote them in bash commands
- **Christ-centered analyses** should focus on how scriptures testify of Jesus Christ, using cross-references from all standard works and modern revelation
