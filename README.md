# DIR Study Hub — GitHub Pages edition

A lightweight, static study dashboard for the TAPMI Diversity, Inclusivity and Rootedness (DIR) course.

## Features
- All 17 chapters from the supplied faculty outline
- Faculty scope notes and topic checklists
- Chapter-specific notes saved in browser local storage
- Faculty-provided video, article and organisation links
- Movie list and case/example prompts
- Application-led practice questions with answer guidance
- Revision flashcards
- Export progress as a JSON file
- Responsive layout for desktop and mobile

## Run locally
No build step or package installation is required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.

For a local web server, you can also run:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`.

## Host on GitHub Pages
1. Create a new GitHub repository, for example `dir-study-hub`.
2. Upload `index.html`, `style.css`, `data.js`, `app.js`, and this README to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site. The URL will appear in the Pages settings.

## Important notes
- This is a static, client-side website. No server or API key is required.
- Progress and notes are stored in the browser's `localStorage` on the device/browser where you use the site. They do not automatically sync across devices.
- Use the **Export** button to download a backup of your progress.
- The syllabus topics and links are organised from the faculty outline supplied by the student. The site does not contain full textbook chapters, full video transcripts, or AI-generated explanations of every topic.
- Some share links are third-party links and may require access or may change over time.
- The flashcards are starter revision aids. Verify textbook-specific definitions and page references against your prescribed book.
- To add content, edit `data.js`. Chapter objects contain `topics`, `focus`, and metadata. Add resource objects to the `resources` array.

## Suggested next upgrades
- Import/export notes
- Search within notes and flashcards
- Add your own textbook summaries and class notes
- Add an AI tutor via a secure backend (never place a private API key in public GitHub code)

## Complete PDF study notes
- Open `study-notes.html` from the dashboard to access searchable text for all 17 chapters of the uploaded Cultural Anthropology end-semester notes PDF.
- Use the search box to find concepts and examples, or expand a chapter to read its complete extracted notes.
- The notes page preserves the scope and source note from the uploaded PDF; use assigned class materials for details that the PDF itself says are not reproduced.
