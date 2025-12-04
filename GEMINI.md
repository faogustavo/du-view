# du-view Project Context

## Overview
**du-view** is a simple, web-based Disk Usage Visualizer. It allows users to visualize their disk usage by parsing the output of the `du` command. The application provides an interactive interface to explore directories and file sizes.

## Technology Stack
- **Core**: HTML5, Vanilla JavaScript (ES6+)
- **Styling**: Tailwind CSS (via CDN)
- **Frameworks**: None (No build step required)

## Key Features
1.  **File Input**: Supports drag-and-drop or file selection for `du` output files.
2.  **Visualization**:
    -   **Stacked Bar Chart**: Visualizes the relative size of subdirectories/files in the current directory.
    -   **File List**: Lists files and directories with their sizes.
3.  **Navigation**:
    -   Clickable bar segments and list items to drill down into directories.
    -   Breadcrumb navigation to easily move back up the directory tree.
4.  **Helper Tools**:
    -   Provides the exact `du` command to generate the compatible output file (`du -h -t 500m ~ > disk-stat.txt`).
    -   "Copy" button to quickly copy the command.

## Usage
1.  Open `index.html` in a modern web browser.
2.  Run the suggested `du` command in your terminal to generate a disk usage report.
3.  Drop the generated text file into the application drop zone.
4.  Explore your disk usage!

## Development
-   Since there is no build step, you can simply edit `index.html` and refresh the browser to see changes.
-   The application logic is contained within the `<script>` tag in `index.html`.
