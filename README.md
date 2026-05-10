# Obsidian Vaults

This repository stores school notes, personal Obsidian vaults, and study material.

It is an active notes backup, not a finished textbook. Some folders overlap because older vaults and cleaner versions are both kept here.

## Quick Start

Open the folder you want as an Obsidian vault.

- Use `main` as the main working vault.
- Use `main/school` for current and future classes.
- Use `code`, `global studies`, `health notes`, or `history 2.0 (no problems)` only when you want those subjects as separate vaults.
- Use GitHub Desktop to review, commit, and push note changes.

## Folder Map

| Folder | What it contains | Use it for |
|---|---|---|
| `main` | The main Obsidian vault. It includes school notes, journal entries, templates, snippets, and Obsidian settings. | Daily note taking and future classes. |
| `code` | A standalone coding vault. It covers HTML, CSS, JavaScript, Python, SQL, React, Node.js, TypeScript, Git, GitHub, and staged learning plans. | Programming study and self-learning. |
| `global studies` | Global studies and civics notes. Current notes cover racial profiling, U.S. amendments, and the Universal Declaration of Human Rights. | Global studies class material. |
| `health notes` | Health class notes. Current notes cover grief, loss, and the stages of grief. | Health class material. |
| `history` | The original AP U.S. History notes folder. It includes early APUSH units, people, laws, events, and concepts. | Older APUSH notes. |
| `history 2.0 (no problems)` | A cleaner and larger APUSH vault. It covers APUSH Units 1 through 4, plus many people, laws, events, parties, cases, and movements. | The better standalone history vault. |
| `md_files_with_images` | Markdown history notes that reference embedded images. | Image-linked history notes. The actual image files are ignored by this repo unless they already exist locally. |

## Main Vault Layout

| Path | What it contains |
|---|---|
| `main/school` | Course pages and subject folders. This is the best place for new classes next year. |
| `main/school/history` | AP U.S. History notes, including APUSH index notes, units, people, events, documents, court cases, and movements. |
| `main/school/math` | Math reference notes. Topics include geometry, topology, compactness, model theory, measure theory, ergodic theory, proof systems, and study guides. |
| `main/school/code` | Coding notes inside the main vault. |
| `main/school/global studies` | Global studies notes inside the main vault. |
| `main/school/health notes` | Health notes inside the main vault. |
| `main/Journal` | Migraine logs and health tracking entries. |
| `main/ztemplate` | Obsidian templates, Templater snippets, Dataview-ready note structures, and CSS snippets. |
| `main/.obsidian` | Obsidian settings for the main vault. |
| `main/ram usage per plugin.md` | Notes about Obsidian plugin RAM usage and startup impact. |

## Current School Notes

These course notes live in `main/school`.

| Note | Subject |
|---|---|
| `AP_US_History_2.md` | AP U.S. History from Reconstruction through the present, with focus on Periods 6 through 9. |
| `Chemistry_Honors.md` | Chemistry Honors lecture and lab topics, including matter, measurement, bonding, reactions, stoichiometry, and lab skills. |
| `Geometry_Honors.md` | Geometry Honors topics, including Euclidean geometry, proofs, lines, angles, transformations, trigonometry, circles, and coordinate geometry. |
| `Health_2_Drivers_Ed.md` | Health 2 and Driver's Education topics, including wellness, mental health, safety, traffic laws, and driving basics. |
| `IB_Design_Technology_1.md` | IB Design Technology topics, including the design cycle, materials, manufacturing, sustainability, and human-centered design. |

## Code Vault

The `code` folder is a separate coding study vault.

Main notes include:

- `Coding - Master Index.md`
- `Beginner Stage.md`
- `Amateur Stage.md`
- `Master Stage.md`
- `HTML.md`
- `CSS.md`
- `JavaScript (JS).md`
- `Python.md`
- `SQL.md`
- `React.md`
- `Node.js.md`
- `TypeScript.md`
- `Git and GitHub.md`

Use this folder when you want coding notes separate from school notes.

## History Notes

There are multiple history folders.

- `history` is the older APUSH folder.
- `history 2.0 (no problems)` is the cleaner standalone APUSH vault.
- `main/school/history` is the history folder inside the main vault.
- `md_files_with_images` stores Markdown versions of history notes that include image embeds.

Do not treat these as four separate classes. They overlap. If you want the cleanest setup, use `main/school/history` for the main vault and `history 2.0 (no problems)` when you want a standalone history vault.

## Templates

Templates live in `main/ztemplate`.

| Path | Purpose |
|---|---|
| `main/ztemplate/Template/subject.md` | Creates a subject page with sections for lectures, tasks, and definitions. |
| `main/ztemplate/Template/lecture.md` | Creates a lecture note linked to a subject. |
| `main/ztemplate/Template/definition.md` | Creates a reusable definition note. |
| `main/ztemplate/Template/assignment.md` | Creates an assignment note. |
| `main/ztemplate/Template/callout.md` | Creates callout-style note blocks. |
| `main/ztemplate/Snippets` | Stores Templater snippets and CSS snippets. |

## Adding New Classes

Use this structure for new classes.

1. Create one course page in `main/school`.
2. Use a clear filename, such as `Physics_Honors.md` or `English_10.md`.
3. Create a matching folder only if the class has many smaller notes.
4. Put the folder under `main/school`, such as `main/school/physics`.
5. Link notes with Obsidian links like `[[Physics_Honors]]`.
6. Keep handouts, images, and PDFs in a clear attachments folder if you decide to track them.

Recommended pattern:

```text
main/
  school/
    New_Class_Name.md
    new_class_name/
      Unit 1.md
      Unit 2.md
      Vocabulary.md
      Review.md
```

## Repo Size

Snapshot checked on May 10, 2026.

| Area | Markdown notes | Total files |
|---|---:|---:|
| `main` | 316 | 429 |
| `history 2.0 (no problems)` | 165 | 241 |
| `md_files_with_images` | 164 | 164 |
| `history` | 75 | 144 |
| `code` | 13 | 74 |
| `global studies` | 2 | 49 |
| `health notes` | 1 | 47 |

The full repository currently has 737 Markdown notes.

## Important Notes

- This repo includes personal health tracking in `main/Journal`. If the GitHub repo is public, that information is public too.
- Images and PDFs are currently ignored by `.gitignore`.
- Notes with image embeds may not render correctly on GitHub or on a new device unless the image files exist locally.
- Several history folders duplicate the same topics. That is useful for backup, but it can make search results messy.
- Some filenames and embedded links may need cleanup over time. Fix duplicates before they turn into broken Obsidian links.

## Backup Workflow

1. Take notes in Obsidian.
2. Open GitHub Desktop.
3. Review changed files.
4. Commit with a clear summary.
5. Push to GitHub.
6. Pull before editing on another device.

## Restoring on a New Device

Clone the repository.

```bash
git clone https://github.com/lrknforexp/obsidian-vaults.git
```

Then open Obsidian and choose `Open folder as vault`.

Use `main` if you want the main school vault.

Use a subject folder if you only want one standalone vault.

## File Rules

The repo currently ignores common attachment formats:

```gitignore
*.png
*.jpg
*.jpeg
*.gif
*.svg
*.webp
*.bmp
*.tiff
*.pdf
```

That keeps the repository smaller, but it also means image embeds can break after cloning. If images matter, track them in a dedicated attachments folder and update `.gitignore`.

