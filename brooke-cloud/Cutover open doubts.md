# Cutover open doubts (from Cloud Brooke prep)

Logged by Brooke Cloud on Sun 2026-11-22, 04:20 CST, at Aaron's request. Source: the Cloud Brooke prep session's own messages (10:14 UTC) and `project-notes/Cutover checklist - local vault to cloud 20261122.md` in `aaronguidewheel/brock-home` (commit f1d5737). The checklist in brock-home is the source of truth. This file is Brooke Cloud's working copy, since Aaron now talks to Brooke Cloud mainly.

## Blockers named by Cloud Brooke prep
1. **`CLAUDE.md` in the repo root.** The cloud session needs its own instructions in brock-home. Today a synced copy sits above the vault, outside GitHub.
2. **Mole password column.** Decide where meter passwords live before mole becomes a Google Sheet. They must not go to a shared cloud sheet. Candidate: a password manager.
3. **Routines to the cloud.** The 11 local scheduled tasks (date-anchor, email digest and scan, control tower, daily and weekly routines) must become cloud routines that read and write through the repo. Every routine must state its time zone (cloud CDT vs Mac Monterrey CST).
4. **Rollback path.** How to go back to local-first within an hour if the cloud fails.

## Accepted risk
- **Parallel-day trial skipped** (Aaron, 2026-11-22, "skip trial"). Routines move without a side-by-side comparison, so each one gets a hand check on its first cloud run.

## Other open items in the checklist (not called blockers)
- Attachments manifest (473 MB stays on Drive, plus a note in the repo listing what exists and where).
- Private local-only folder: decide where it lives after decommissioning.
- Live memory store for the cloud session (the repo only holds backup v39.0.0).
- Skills installed where the cloud session loads them (copies sit in `system/skills`).
- Directive rules that mention local paths, the Mac clock and the browser.
- Writer rule (who commits, how often, conflicts): draft only.
- Mailbox transport through git, replacing Drive.
- Connector checks from the cloud: Gmail, Calendar, Slack, Granola, Drive, Sheets, Atlassian.
- `Today.md` written by a cloud routine.
- Meter and browser work stays on the Mac: decide what "decommissioned" means.
- Full backup and restore test of the cloud copy.
- Aaron signs the cutover (gate G5).

## Extra doubts from Cloud Brooke prep (Sun 2026-11-22, about 04:25 CST)
Sent directly to Brooke Cloud. All are in the checklist; these are the ones it wants watched.
1. **Memory store.** Live memory sits on the Mac. The repo only has a backup (agent-memory 41.0.0). Brooke Cloud has no live store yet.
2. **Time zone.** The cloud scheduler runs on CDT, the Mac on Monterrey CST. Every routine must state its zone.
3. **Session board and messaging.** Control tower and cross-session messages only work between local sessions. Decide the cloud equivalent. (Observed: Brooke Cloud can message local sessions directly; local sessions cannot reach Brooke Cloud.)
4. **Mailbox transport.** Brooke Cloud can't edit Drive files it didn't create, or rewrite its own, so the mailbox moves to git or direct messages.
5. **Connector read tests from Brooke Cloud.** Already used successfully in this session: Google Drive (read, create), Google Calendar (read, create), Granola (not yet), Gmail (not yet), Google Sheets (not yet), Slack (not yet), Atlassian (not yet).
6. **Meter and browser work stays on the Mac.**
7. **Meter passwords** need a home outside any repo.
8. **Backup and restore test**, plus rollback within an hour.

Writer rule unchanged: Cloud Brooke prep is the only committer to brock-home during the freeze, until Aaron says otherwise.

## Decision log
- **Sun 2026-11-22 04:17 CST, Aaron:** "your memory is now the main one. local vault is decomissioned and archived starting now." Brooke Main and Cloud Brooke prep told to stop writing to the local vault; archive actions on the Mac wait for Aaron's go in those sessions. Open: who commits to brock-home now.
