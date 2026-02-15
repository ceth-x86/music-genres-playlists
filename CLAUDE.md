# Data Project

## genres-playlists

Playlist files in current catalog are markdown documents with curated track lists organized by genre.

### Format

Each entry follows this structure:

```
**Artist — Track Title (Album, Year)**
Description text in plain (non-bold) format.
```

- Entries are grouped under `## Section headers` (typically by era/period)
- No numbering — entries are a plain sequential list
- Header line (artist, track, album, year) is **bold**
- Description is regular text on the next line
- Blank line between entries

### README.md structure

README.md headers must follow the hierarchy from `classification.yaml`:
- Top-level YAML categories become `##` headers
- Subcategories become `###` headers
- Playlists are listed as links under the most specific matching header

When adding a new playlist to README.md, find its position in `classification.yaml` and place it under the correct parent/subcategory headers, creating new headers if needed.

### Converting from table format

When converting a markdown table to this list format:
- Artist goes first, then em dash `—`, then track title
- Album and year go in parentheses after the track
- Rationale/description becomes the plain-text line below
- Drop the `#` column (no numbering)
