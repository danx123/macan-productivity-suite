## Macan Productivity Suite
Macan Productivity Suite is a comprehensive, integrated collection of desktop applications designed to streamline your workflow and enhance operational efficiency. This suite provides a robust set of tools engineered for daily computational, archival, and document management tasks.
---
## Showcase
<img width="1728" height="2544" alt="macan-productivity-suite-github" src="https://github.com/user-attachments/assets/4615a8e7-da13-4818-b4c7-2fe78858db6c" />

## Core Components
The suite includes five powerful applications, each tailored for a specific productivity function:
1. Macan Archiver
A high-compression file archiving utility. It features support for a proprietary .mcn format, alongside full compatibility with standard archives including 7z, ZIP, RAR, TAR, GZIP, and more.
2. Macan Count Pro
An advanced calculator designed for both simple and complex computations. It features standard, scientific, and programming modes to handle a wide array of mathematical tasks.
3. Macan Notes Pro
A versatile, multi-format text and code editor.
Broad File Support: Provides native support for .txt, .md (Markdown), .py, .html, and .docx.
Export Functionality: Includes a robust Export to PDF feature for seamless document conversion and sharing.
4. Macan Reader
A lightweight, fast, and reliable PDF viewer. It is optimized for high performance, minimal resource consumption, and a clean, distraction-free reading experience.
5. Macan Download Manager
A sophisticated tool for managing, scheduling, and accelerating your file downloads. It ensures download integrity, supports pausing/resuming, and handles multiple download streams efficiently.
---
## Getting Started
This product is distributed as a binary-only release. No compilation or setup scripts are required.
Navigate to the Releases page of this repository.
Download the latest release asset appropriate for your operating system.
Extract the archive (if applicable) and launch the application.
---
## Changelog v2.3.0 (10-11-2025)
1. Macan Notes Pro v4.7.0 - 5.0.0
   🚀 New Features
Added "Paste as Plain Text" Action:

Introduced a new "Paste as Plain Text" feature, accessible from the Edit menu or via the Ctrl+Shift+V shortcut.

This allows users to paste content from the clipboard while stripping all external formatting.

This resolves an issue where content pasted from external sources (like web browsers) would retain its original styling (e.g., black text in a dark theme), ensuring pasted text always respects the application's current theme.

🛠️ Improvements & Fixes
Enabled Rich Text Formatting Persistence for HTML:

Modified the file I/O logic to provide support for saving and loading rich text formatting (e.g., bold, italics, lists, and text alignment).

Save Logic: The application now serializes the editor's content to HTML when the file extension is .html or .htm. All other formats are saved as plain text as before.

Load Logic: The application now correctly deserializes .html and .htm files, restoring all rich text formatting when a file is opened.
---
## License & Copyright

Copyright © 2025 - Danx Exodus - Macan Angkasa. All rights reserved.
Unauthorized copying, distribution, or modification of this software is strictly prohibited.
