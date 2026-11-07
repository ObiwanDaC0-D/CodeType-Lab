# CodeType Lab

CodeType Lab helps programmers develop faster, more accurate typing through exercises involving code, symbols, operators, and indentation. It combines a distraction-reduced practice interface with measurable typing sessions, analytics, and self-directed experiments. Browser input telemetry has limitations and should not be interpreted as laboratory-grade keystroke measurement.

**At a glance:** A focused typing practice laboratory for programmers, combining realistic code and syntax drills, speed and accuracy feedback, training analytics, and repeatable performance experiments.

---

# CodeType Lab

A free, standalone typing trainer built for programmers. Practice real code, punctuation, operators, and indentation in a distraction-free editor-inspired interface.

## Version 11.0 — Input integrity and learning reliability\n\n- Detect unmeasured bulk insertions, including paste-like edits, and exclude those sessions from experimental trials\n- Handle IME composition events without treating intermediate text as ordinary keystrokes\n- Clear completion feedback when an assessment is ineligible\n- Preserve all existing training, focus, analytics, and backup functionality\n\n**Known limitation:** Browser input events are not physical keystroke telemetry; single-character paste/autocorrect and certain complex edits can still be difficult to distinguish. Cumulative accuracy is an approximation.\n\n## Version 10.0 — Performance and usability\n\n- Reuse target-character DOM nodes while typing instead of rebuilding the full target markup\n- Reduce timer-driven metrics refreshes from 100 ms to 250 ms\n- Add a persistent distraction-reduced Focus mode\n- Add quick navigation to practice, analytics, experiments, and backup\n- Preserve all existing training and analytics features\n\n**Audit priorities still open:** Interactive cross-browser testing, long-session profiling, improving the measurement model for corrections/paste, and stronger experimental study design.\n\n## Version 9.0 — Quality and reliability\n\n- Automated Node regression tests run on pushes and pull requests via GitHub Actions\n- Syntax, duplicate-ID, element-reference, data-normalization, and accessibility smoke checks\n- Better keyboard focus visibility, labelled input, live status announcements, reduced-motion support\n- Versioned JSON backup and restore with explicit replacement confirmation\n- Local-storage write failures are surfaced instead of silently ignored\n- Legacy local data is normalized on load, with invalid settings reset to safe defaults\n\n**Run checks locally:** `node --test tests/quality.test.mjs` (Node.js 22+). The automated suite is a static/regression suite, not a substitute for interactive browser testing.\n\n## Version 8.0\n\n- Cumulative single-character insertion accuracy alongside current-text accuracy\n- Per-session typing and error counters\n- Corrected per-character timing attribution and timing-sample quality labels\n- Optional strict assessment eligibility requiring at least 95% cumulative accuracy\n- Session-only counter reset without erasing history\n- Browser input events are approximate; paste, IME, autocorrect, and physical keydown timings are not fully measured\n\n## Version 7.0\n\n- Research dashboard with session-level WPM and accuracy charts\n- Language, mode, and 7/30/90-day or all-time filters\n- Median WPM, accuracy, session count, and practice-time summaries\n- Early-versus-recent descriptive comparisons and A/B assessment summaries\n- Filtered session CSV export\n\n## Version 6.0\n\n- Repeatable fixed-snippet assessments with 1, 3, or 5 trials\n- Median WPM and speed-range summaries with adjustable accuracy thresholds\n- Trial-level CSV export for analysis\n- Corrected curriculum mastery attribution before level advancement\n- Assessment results remain observational, not causal evidence\n\n## Version 5.0\n\n- Baseline and follow-up assessments using a fixed code snippet\n- Compare adaptive accuracy training (A) with key-transition practice (B)\n- Retention assessment unlocked 24 hours after follow-up\n- Per-approach WPM comparisons and complete local JSON data export\n- Results are observational and do not establish causal effectiveness\n\n## Version 4.0\n\n- Keyboard-layout heatmaps (QWERTY, Dvorak, Colemak visual references)\n- Approximate key-pair timing and error analysis\n- Targeted key-transition drills with speed/error/balanced emphasis\n- Curriculum mastery attempt and pass counts\n\n## Version 3.0\n\n- Five-stage programming curriculum with 95%-accuracy progression\n- Recent-session WPM and accuracy visualization\n- Daily training goals and progress tracking\n- Personalized suggested practice sequence\n- Existing local data remains available in the browser\n\n## Version 2.0\n\n- Personalized coaching dashboard with weakest-character and coding-pattern indicators\n- Approximate per-character input intervals (excluding pastes and bulk edits)\n- Adaptive exercises with balanced, accuracy-first, or speed-first emphasis\n- Focused coding-pattern drills for brackets, operators, strings, functions, and indentation\n- All measurements remain local in your browser\n\n## Features

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
