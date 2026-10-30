# Paste this into a new Claude chat

```
I'm continuing a finished university project: two finance case decks (Group 10, HBS Case 1 — Jaguar Land Rover bond refinancing, and UK Gilts) built as Claude Slides decks. Everything is already done, checked and approved. Your job is to restore it in my account, not redo it.

1. Download and unpack the project (do not edit the original zip):
   mkdir -p ~/g10 && cd ~/g10 && curl -L -o g10.zip "https://github.com/Ahnafahad/group10-hbs-case1-decks/raw/main/Group10-HBS-Case1-PUBLIC-2026-10-30.zip" && unzip -q g10.zip
   If the download is blocked in your environment, tell me in one line and I will attach the zip instead.
2. Read proj/START_HERE.md, then proj/CLAUDE.md ("Hard rules" and "Standing rules from the user" are the rubric and override everything), proj/review/PROGRESS.md (my feedback word for word, newest first) and proj/DESIGN.md.
3. Run: cd ~/g10/proj && bash resume.sh. It installs what it needs, runs both calculation files (every number is asserted), rebuilds both decks from the build scripts and render-checks every slide. It must print READY. If anything fails, fix only that and tell me.
4. Publish both decks as NEW Claude Slides decks in my account: create one Slides artifact per deck from the "Slides" artifact type (titles "Jaguar Land Rover: Group 10 case deck" and "UK Gilts: Group 10 case deck"), then publish decks/<case>/project/deck.json plus every project/slides/<id>.html listed in its "order", with root = decks/<case>. Follow proj/SLIDES_PUBLISHING.md exactly. Max 255 files and 64 MB per call (each deck fits in one call). Do not change the slide files when publishing.
5. Reply with the two deck links and one line each. Then stop and wait.

Rules: do NOT re-read the case, re-derive the analysis, redesign, or re-review anything already approved. Numbers only from work/<case>/calcs.py; facts only from work/<case>/sources*.md; never cite the teaching notes. Body text at least 18pt (36px), footers 12pt. Cover details and the team slide stay as marked placeholders until I supply them. If I later ask for changes: write my feedback word for word into review/PROGRESS.md first, edit the build script (build/jlr_s1..s7.py or build/gilt_a..e.py), rebuild, run build/render.py, and republish only the changed slides. Ask me questions only if genuinely blocked, as multiple choice in simple words with a recommendation. Be fast and token-efficient.
```

Note: the HBS case files and CFA notes are not in the public zip. They are only needed to re-read the case, not to rebuild or edit the decks.
