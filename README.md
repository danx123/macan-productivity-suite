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
## Changelog v2.4.0 
1. Macan Reader v4.0.0 - 4.5.0
   ✨ New Features
Continuous View Mode: Users can now toggle between the default "Single Page" view and a new "Continuous" view (Ctrl+7). This mode renders all pages in a single vertical column, allowing for smooth scrolling through the entire document without clicking "Next" or "Previous."
Toolbar Toggle: A new "Continuous View" icon has been added to the main toolbar to easily switch between view modes.
🚀 Improvements & Fixes
Virtual Page Rendering (Lazy Loading): To ensure high performance in Continuous View, only the pages currently visible (plus a small buffer) are rendered. Pages that scroll out of view are cleared from memory, keeping memory usage low even for large documents.
FIXED: Lazy Loading Render Bug: Resolved a critical bug where the lazy loading mechanism would fail to render pages beyond the initial view (often stopping after 1-2 pages). All pages now correctly load as the user scrolls.
Enhanced Tool Compatibility:
Zoom: Zooming (Ctrl++/Ctrl+-, slider) now works perfectly in Continuous View, resizing all pages and recalculating the scroll layout on the fly.
Pan Tool: The Pan tool (Hand icon) is fully functional across all pages in Continuous View.
Search: Highlighting a search result (Ctrl+F) now correctly navigates to the corresponding page and scrolls it into view in both Single and Continuous modes.
Go to Page: Jumping to a page (via Ctrl+G, thumbnails, or bookmarks) now instantly scrolls to the correct page's position in Continuous View.
UI Smarts: The "Fit to Page" (Ctrl+9) action is now intelligently disabled in Continuous View, as it is only applicable to Single Page mode. "Fit to Width" (Ctrl+8) remains functional in both modes.

2. Macan Archiver v4.5.0 - 4.7.0
   🐞 Fixed * Addressed a critical bug in the "Copy Selected" (context menu) functionality where attempting to copy multiple items from an archive would fail unpredictably. * The bug could cause either **only one item** to be copied (despite selecting multiple) or, in some cases, the **entire archive's contents** to be extracted and copied, ignoring the user's selection. * Reworked the `_copy_selected_files_to_clipboard` method to be significantly more robust. Instead of passing filenames as command-line arguments (which caused the failure), the function now: 1. Writes the list of selected files to a temporary `listfile.txt`. 2. Calls `7z.exe` using the `@<listfile>` switch, which reliably handles any number of files. * The "Copy Selected" action now correctly extracts *only* the chosen files/folders to the temporary directory, ensuring that pasting into Windows Explorer works as expected.
---
## License & Copyright

Copyright © 2025 - Danx Exodus - Macan Angkasa. All rights reserved.
Unauthorized copying, distribution, or modification of this software is strictly prohibited.
