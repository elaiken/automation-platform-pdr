# Directions

## Local Structure
- README.md: repository overview
- docs/PDR.md: product design requirements (source of truth)
- docs/DIRECTIONS.md: local workflow and documentation conventions

## Documentation Conventions
- Keep language simple and direct.
- Add dates to major updates in PDR as a note in the section being updated.
- Prefer short sections over long paragraphs.

## Updating the PDR
1) Edit the relevant section in docs/PDR.md.
2) Add a short note with the update date and reason.
3) Keep changes aligned with the shared core + industry layer architecture.

## GitHub Workflow (when ready)
1) Initialize the repo: `git init`
2) Add files: `git add .`
3) Commit: `git commit -m "Add initial PDR and docs"`
4) Create a GitHub repo and add remote: `git remote add origin <repo-url>`
5) Push: `git push -u origin main`

## Suggested Next Docs
- docs/ARCHITECTURE.md (platform overview)
- docs/INDUSTRY-PACKS.md (per-industry feature sets)
- docs/SECURITY.md (audit, retention, access control)
