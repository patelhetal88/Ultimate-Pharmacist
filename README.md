# Ultimate Pharmacist – PEBC Study Guide

An iPhone-focused Canadian pharmacy study app with English and Hindi audio. Ontario is the default, with all ten Canadian provinces available. This is the **all-topic review edition**, prepared September 19, 2026.

## What works

- 150 concise topic reviews, internal search, personal notes, bookmarks and rapid review.
- 300 playable MP3s: every topic in English and Hindi. Approximately 130 minutes in English and 86 minutes in Hindi.
- Searchable audio chapters, subject filters, transcripts, continuous playback, saved positions, playback speed, sleep timer and media controls.
- 226 original formative questions with explanations for all four options. Custom topic, competency and difficulty sessions; saved attempts; mistake review.
- A 200-question, 260-minute timed practice set using the published PEBC Part I competency proportions. The timer continues when you leave, and explanations appear after submission.
- 20 guided or seven-minute OSCE exercises, self-reflection checklists and optional device-local voice recording.
- Nine calculation tools with worked solutions, unit checking and practice problems; four prescription-discrepancy exercises.
- Spaced flashcards, a 20-subcompetency personal checklist, progress and a flexible final-seven-days review plan.
- Provincial regulator links and an introductory Ontario JEP pathway.
- A separate **Official exam samples** section linking to released PEBC MCQ/OSCE materials, sample-exam information and Ontario JEP samples. These are external official resources, not a ten-year archive of actual exam papers or part of the app's original question bank.
- Larger text, light/dark appearance, keyboard navigation, progress backup/restore, installable app icons and an offline study shell.
- Optional external Gemini link. No ChatGPT search, API keys or automatic transfer of notes.
- Instructions for user-created Siri shortcuts that open the app or Hindi audio.

## Coverage and review status

Every listed topic has a short review and bilingual audio. This **does not mean every licensing examination or the complete originally planned course is covered**. Comprehensive treatment chapters, independently reviewed dose tables, a complete drug master library and complete provincial law/exam courses remain in development. The drug area currently contains eight study-index entries.

Questions and OSCE exercises are original educational material, not official PEBC items. The practice bank has not been independently clinically reviewed or calibrated to PEBC difficulty. Exam length and blueprint proportions alone do not validate an exam simulation. Progress is a study record, not a prediction of passing.

Recordings use synthetic Microsoft speech voices: en-CA-LiamNeural and hi-IN-MadhurNeural. Hindi conveys core ideas rather than a word-for-word translation. Clinical, translation and pronunciation review by qualified independent reviewers is pending. Further-reading links do not certify every statement. Verify current clinical and legal information in authoritative Canadian references.

This independent study companion is not affiliated with PEBC or a regulator and is not a patient-specific prescribing tool. Provincial selection changes the study context; it does not establish registration eligibility.

## Use on iPhone

After HTTPS hosting is enabled, open the app in Safari and use **Share → Add to Home Screen**. Settings includes Siri shortcut instructions. These shortcuts open a URL; they do not provide native Siri playback commands. Safari may require a tap to start audio. Physical-iPhone checks of installation, recording, background playback and lock-screen chapter transitions remain pending.

Audio requires a connection unless the chapter has been downloaded. Audio is intentionally excluded from the offline cache. Downloaded MP3s can be played separately in a compatible player.

## Privacy and recovery

Notes, preferences and progress stay in this browser's local storage. They do not sync between devices. Export a backup before clearing browser data. Voice recordings remain in memory until downloaded or deleted; refreshing can discard them. No recording upload is implemented. Gemini opens separately and receives no notes automatically.

Public hosting serves the app, educational text and course recordings. The hosting provider receives normal web requests. Public source does not contain a user's personal progress or recordings.

## Run and publish

The app is plain HTML, CSS and JavaScript. Serve the contents of `dist/` over HTTP for local use, or HTTPS for production. Use a server with HTTP byte-range support for audio seeking. The accompanying release ZIP places the contents of `dist/` at its root, ready for GitHub Pages branch/root hosting. The local source folder retains `dist/` for development.

For GitHub Pages, publish the ZIP's extracted files at the repository root, including the `audio/` folder and `.nojekyll`; select the main branch and root folder in Pages settings. Never upload `.git/`, `.openai/`, progress backups or personal recordings. All app asset paths are relative and have been checked beneath `/Ultimate-Pharmacist/`.

`data.js` contains course data and MP3 metadata, `app.js` contains interaction and persistence, and `sw.js` contains the offline shell. Increment the service-worker cache identifier when publishing changes. Lucide's license is in `ICONS-LICENSE.txt`.

## Validation

Automated browser checks cover mobile and desktop layouts (320, 390 and 1280 pixels), 200% text, navigation, all province options, search, escaped notes, progress persistence and recovery, offline lessons, question locking and submission, exact full-length competency counts, timer persistence, new OSCE debriefs, calculations, flashcards, audio filtering/language switching/seeking/resume and settings. All 300 MP3s passed full-file decoding and duration checks. This is technical verification, not clinical or physical-device certification.

Exam-format references: [PEBC blueprint](https://pebc.ca/pharmacists/qualifying-examination/preparing-for-the-examination/examination-blueprint/) and [PEBC FAQ](https://pebc.ca/faq/). Ontario requirements: [OCP JEP](https://ocpinfo.com/applicants/registration-requirements/jurisprudence-ethics-and-professionalism-exam/).
