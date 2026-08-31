# How-to-Create-an-Excellent-and-Professional-Software

# The Great Software Quest

An interactive, one-file learning handbook about building software people love
and trust.

Author credit: **A.R.Cabornay**

## Files

- index.html — the complete guide; its HTML, CSS, learning content, diagrams,
  quizzes, simulations, accessibility controls, adaptive route assessment,
  mastery checkpoints, five-mission capstone, study drawer, 100-card spaced
  review bank, and local progress system are contained in this one file.
- supabase_setup.sql — tables, grants, Row Level Security policies, triggers,
  and self-service account deletion for optional cloud backup and feedback.
- LICENSE-CONTENT.txt — Creative Commons Attribution 4.0 notice for the
  educational content.
- LICENSE-CODE.txt — MIT License for the website source code.
- VERIFICATION_REPORT.md — completed checks and the remaining launch checks.

## Important offline behavior

The guide works offline when index.html is downloaded and opened. Progress is
saved locally first, including route results, notes, bookmarks, capstone drafts,
checkpoint results, and spaced-review history. Cloud backup, email sign-in,
feedback submission, and external source links naturally require an internet
connection.

An exactly one-file website cannot register the separate same-origin service
worker required for installable, visit-once-then-reopen-offline PWA behavior.
That limitation is intentional because the requested deliverable is one HTML
file.

## Supabase setup

1. Open the Supabase SQL Editor for the configured project.
2. Run all of supabase_setup.sql.
3. In Authentication settings, enable Email, Anonymous Sign-Ins, and Manual
   Linking.
4. Put the final GitHub Pages address in Site URL and Redirect URLs.
5. Configure production SMTP before relying on cross-device email sign-in.
6. Before a large public launch, add CAPTCHA or Turnstile protection as
   recommended by Supabase for anonymous sign-ins.
7. Run Supabase's Security Advisor and confirm both Quest tables have RLS.

The publishable key is expected to be visible in browser code. Security depends
on database grants and Row Level Security. Never place a service_role or secret
key in index.html.

## Privacy launch checklist

The guide uses local-only progress by default. Cloud backup is opt-in.

Before publishing:

1. Search index.html for OWNER_PRIVACY_CONTACT and enter a real contact method.
2. Search for OWNER_DATA_REGION and describe the Supabase project region.
3. Search for OWNER_RETENTION_PERIOD and state the actual anonymous-account retention rule.
4. Confirm the retention period in the privacy dialog matches the actual
   operating practice.
5. Confirm how data-subject requests will be received and handled.
6. If children may use the guide, keep cloud backup optional and instruct them
   to involve a parent or guardian when local law requires it.
7. Review the deployment with a qualified privacy professional. The guide
   implements privacy-oriented defaults, but a software artifact alone cannot
   guarantee legal compliance in every country.

## Publish with GitHub Pages

1. Create or open a GitHub repository.
2. Upload the contents of this quest folder to the repository root.
3. Keep the main guide named index.html.
4. In GitHub: Settings → Pages → Deploy from a branch.
5. Select the publishing branch and / (root).
6. Open the published address and test local progress, keyboard navigation,
   mobile layout, optional cloud sync, email return links, feedback, and data
   deletion.

## Recommended final tests

- Complete one chapter and reload the page.
- Answer a quiz using only the keyboard.
- Complete the eight-question route finder and confirm every chapter remains open.
- Make one correct and one incorrect quiz choice; only the mistake should show
  an explanation.
- Start a Memory Hall session and confirm it contains exactly ten questions.
- Answer a review card incorrectly, reload, and confirm it is due again soon.
- Save a chapter note and bookmark, then export and import the learning JSON.
- Complete one mastery gate and one capstone attempt-before-coaching flow.
- Step through all six visual explanations using Back, Next, and Replay.
- Download index.html, disconnect from the internet, and open it.
- Enable cloud backup and verify a row appears in quest_progress.
- Try to read another test user's row; RLS must block it.
- Link an email, sign in on a second browser, and verify merged progress.
- Submit and delete feedback.
- Delete the cloud account and confirm Quest rows cascade away.
- Test at 200% zoom, high contrast, reduced motion, and a narrow phone width.

## License

The learning content is licensed under CC BY 4.0, with attribution to
A.R.Cabornay. The website code is licensed under MIT. See the two license files
for details.
