# CodeType Lab

A free, standalone typing trainer built for programmers. Practice real code, punctuation, operators, and indentation in a distraction-free editor-inspired interface.

## Version 2.0\n\n- Personalized coaching dashboard with weakest-character and coding-pattern indicators\n- Approximate per-character input intervals (excluding pastes and bulk edits)\n- Adaptive exercises with balanced, accuracy-first, or speed-first emphasis\n- Focused coding-pattern drills for brackets, operators, strings, functions, and indentation\n- All measurements remain local in your browser\n\n## Features

- Practice JavaScript, Python, TypeScript, HTML, CSS, SQL, and JSON
- Real-code exercises, symbol drills, and adaptive practice
- Custom code snippets
- WPM, accuracy, error count, elapsed time, and completion progress
- 30-second, 60-second, 2-minute, or full-snippet sessions
- Character difficulty visualization
- Local progress history and CSV export
- Responsive layout and keyboard-friendly controls
- No dependencies, backend, accounts, or tracking

## Run locally

Open `index.html` in a modern browser.

## Deploy on GitHub Pages

1. Open the repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/(root)**, then save.
4. Visit the Pages URL GitHub provides after deployment.

## Notes

WPM is calculated using five correct characters per word and elapsed time. Accuracy measures the percentage of currently entered characters matching the target at their positions. The adaptive character map tracks incorrect character entries locally. This is a training aid, not a standardized assessment.

Progress is stored in browser localStorage, so it does not sync across browsers or devices. Export CSV to keep a copy.

## Privacy

No external services or analytics. The app does not send typed code anywhere. Avoid pasting secrets into any software you do not trust.

## License

No license has been added yet. The repository owner can choose one before inviting external contributions.
