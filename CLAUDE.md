# Draft fanarchive

A fanfic archive on the AT Protocol. See `readme.md` for the repo layout and `notes/` for design notes (LaTeX).

## AT Protocol context to pull

The project is in the ideation phase. Whenever a design question touches non-public data, read access, audiences, or who may write into whose data, fetch these before reasoning from memory. Both are moving targets, so re-fetch rather than relying on earlier summaries.

- **Spaces / permissioned data proposal:** https://github.com/bluesky-social/proposals/tree/main/0016-permissioned-data
  The directory is still named "permissioned-data", but the feature is now called atproto Spaces.
- **"Reintroducing Spaces"** (Daniel Holmgren, 2026-08-27): https://dholms.leaflet.pub/3mu3p3ldwrc26
  A motivation and design-rationale post. Key points for us:
  - A Space is a shared social context. Each record lives in exactly one Space, which has a single owner and a single modality. Everyone with access sees the same view.
  - Spaces are described as "mini atprotos", so moderation, migration and app roles follow existing atproto patterns.
  - It deliberately rejects "Circles" (content first, audience attached). Its postulate: a record can be safely and legibly shared with two circles only if both were created by the same entity and share a modality.
  - Per-record audiences, such as sharing each recipe with different people, got less design focus. The suggested workaround is shared Spaces with app-level access logic.
  - Spaces are in alpha, and the author is asking for feedback.

## Where this is already referenced

- `notes/WorksInCollection/ReadingSequences.tex`, Permissions section: footnote on the tension between Spaces (which govern reads, not writes) and enforcing reference policy at the AppView.
- `notes/WorksInCollection/GroupsAndSequences.tex`, Permissions section: footnote on reading permissions.

Both notes are written against the moving proposal, which is fine for now. Recheck them against the current text before anything is finalized.
