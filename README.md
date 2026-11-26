# Kindle Notes to Obsidian Converter

Python utility which convert Kindle highlights and notes into Obsidian-friendly Markdown files.

## How to Use

1.  **Export your notes:** Get your notes from your Kindle device. This is usually a file named `My Clippings.txt`.
2.  **Place the file:** Put your `My Clippings.txt` file in the same directory as the script, and rename it to `kindle_highlights.txt`.
3.  **Run the script:**
    ```bash
    python main.py
    ```
4.  **Find your notes:** The script will create a new folder called `obsidian_notes` with your notes converted to Markdown files.

## Example

### Input (`kindle_highlights.txt`)

```
Psychocybernetics (Maxwell Maltz)
- Your Highlight at location 617-619 | Added on Tuesday, March 4, 2025 5:28:36 PM

The goals of our creative mechanism are PSYCHOLOGICAL IMAGES or mental pictures, which we create through IMAGINATION.
==========
Building a Second Brain (Tiago Forte)
- Your Highlight on page 42 | Location 550-551 | Added on Monday, June 16, 2025 12:30:51 AM

To guide you in the process of creating your own Second Brain, I've developed a simple, intuitive four-part method called "CODE"—Capture; Organize; Distill; Express.
==========
```

### Output (`obsidian_notes/Psychocybernetics.md`)

```markdown
---
title: Psychocybernetics
author: Maxwell Maltz
type: book
tags: 
  - book
  - highlights
date: 2025-10-01
---

# Psychocybernetics

**Author:** Maxwell Maltz

---

## Notes and Highlights

### 📌 Highlight #1

**Location:** 617-619
**Date:** Tuesday, March 4, 2025 5:28:36 PM

> The goals of our creative mechanism are PSYCHOLOGICAL IMAGES or mental pictures, which we create through IMAGINATION.
```
