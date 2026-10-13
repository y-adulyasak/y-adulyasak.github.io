# Yossiri Adulyasak — website

| File | Page |
|---|---|
| `index.html` | Home |
| `cv.html` | Brief CV |
| `publications.html` | Publications (filter by application, domain, method, type, journal) |
| `team.html` | Research team |
| `links.html` | Links |


## Publish on GitHub Pages

1. Create a public repository named `y-adulyasak.github.io`.
2. Upload all the files in this folder (Add file → Upload files) and commit.
3. Settings → Pages → Build and deployment → Deploy from a branch → `main` / root.
4. The site appears at `https://y-adulyasak.github.io/` after a minute or two.

## Show the pages inside Google Sites

For each Google Sites page (Home, Brief CV, Publications, …):

1. Insert → Embed → **By URL**, paste the GitHub Pages address of the matching page,
   e.g. `https://y-adulyasak.github.io/publications.html`, choose **Whole page**, Insert.
2. Drag the embed box's bottom edge down so the page has room.

When embedded, the pages hide their own menu (Google Sites supplies it) and open every link in a new tab.

## Editing

Edit the files on GitHub (open the file, click the pencil icon, change the text, Commit changes).
The live site and every Google Sites embed update within a minute or two.
Content inside the embeds can't be edited from the Google Sites editor.

- **Home, Brief CV, Research team, Links:** plain HTML text and lists. To add a person or an award,
  copy an existing `<li> … </li>` line and change the text.
- **Publications:** the `PUBS` list near the bottom of `publications.html`; instructions are in the comment above it.
  Each entry has `app` (application: `prodinv`, `transport`, `network`, `demand`, `platforms`, `health`, `fundamental`),
  `dm` (methodological domain: `or`, `ml`, or both) and `m` (method: `unc`, `algo`, `robust`, `rl`, `sup`, `unsup`,
  `llm`, `aiapp`, `emp`). Add `ind: true` to list a paper under "Industrial collaborations".
  A method appears in the filter only once at least one paper uses it (e.g. `llm`).
  The UTD24 and ML/AI conference groups come from the `utd` and `ai` flags on each venue in `VENUES`,
  so a new paper in, say, *Operations Research* is marked automatically.
- **Order of the filters:** every filter list (applications, domains, methods, types, journals) appears in the
  order its lines are written in the file. To reorder journals, move lines up or down inside `VENUES`;
  `VENUES_SHOWN` sets how many appear before "Show all". To rename one, change its `s:` (short label) or `f:` (full name).
