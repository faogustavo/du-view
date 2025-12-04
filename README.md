# du-view

A simple, elegant web-based **Disk Usage Visualizer** that helps you understand your disk space usage through interactive visualizations.

## Features

- **Interactive Visualizations**: Stacked bar charts and file lists to explore your disk usage
- **Easy Navigation**: Click on directories to drill down, use breadcrumbs to navigate back
- **Beautiful Dark UI**: Modern terminal-inspired design with smooth animations
- **Customizable Commands**: Configure `du` command options through an intuitive interface
- **Copy to Clipboard**: Quickly copy commands and file paths
- **No Build Required**: Pure HTML, CSS, and JavaScript - just open and use

## Usage

1. **Generate disk usage data**:
   ```bash
   du -h -t 500m ~ > disk-stat.txt
   ```

2. **Open the app**:
   - Simply open `index.html` in your web browser
   - Or serve it locally:
     ```bash
     npx serve .
     ```

3. **Load your data**:
   - Drag and drop the `disk-stat.txt` file into the drop zone
   - Or click to select the file

4. **Explore**:
   - Click on bar segments or list items to navigate into directories
   - Use breadcrumbs to go back up the directory tree
   - Customize the `du` command using the settings panel

## Customization

Click the settings icon (⚙️) next to the command to customize:

- **Flags**: `-h` (human-readable), `-s` (summarize), `-a` (all files)
- **Path**: Target directory to analyze
- **Max Depth**: Limit directory depth with `-d` flag
- **Threshold**: Filter files/directories by size with `-t` flag

The command updates automatically as you change options!

## Technology Stack

- **HTML5**: Structure and semantics
- **Vanilla JavaScript**: All logic, no frameworks needed
- **Tailwind CSS**: Styling via CDN
- **Built with**: [Antigravity](https://antigravity.google/) - Google's AI-powered coding assistant
- **Powered by**: Gemini 2.0 Flash Experimental

## Development

No build step required! Just edit `index.html` and refresh your browser.

```bash
# Serve locally for development
npx serve .
```

## Project Structure

```
du-view/
├── index.html          # Main application (all-in-one file)
├── README.md          # This file
└── .agent/            # Antigravity workflows and context
    └── workflows/
```

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

MIT License - feel free to use this project however you'd like!

---

**Built with [Antigravity](https://antigravity.google/)**
