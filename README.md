# files3d

Explore a GitHub repository as a building. Each folder is a floor; opening a folder builds its floor up and to the right of its parent, like Miller columns in 3D, so the parent stays in view.

## Use it

Open `index.html` in a browser (or serve the repository with GitHub Pages) and enter a repository: `owner/repo`, a `github.com/owner/repo` link, or a link to a branch or folder such as `github.com/owner/repo/tree/main/src`. You can also link straight to one with `index.html?repo=owner/repo`.

- **Click a folder** to open it on the right. Opening another folder from the same parent puts it on the same level; floors never swap places. Click one that is already open to make it current.
- **Click a file** to preview it. The bar at the bottom links to it on GitHub.
- **× on a floor** closes it. **Esc** goes back one level.
- **Sort** by name, size or date, in either direction, with folders first or mixed in.
- **Layouts:** Terraces (one row per item), Tiles (a grid) or Ruler (items placed along a size, date or name scale).
- **View:** five camera angles, from isometric to near-plan, with labels painted on the floor in perspective or facing the screen.
- **Pan** by dragging or two-finger scrolling, **zoom** with the wheel or a pinch, and **double-click empty space** to reset the view.

## GitHub limits

The whole file tree loads in two requests. Modification dates are not part of that listing, so they are fetched only when you sort by date, one request per item on the floors you have open. Without a token GitHub allows 60 requests an hour; a personal access token (the "GitHub token" menu) raises that to 5,000 and gives access to private repositories. The token is stored in your browser only and sent only to `api.github.com`.

Repositories with more than about 100,000 files come back truncated from GitHub; the page says so when that happens. Each floor draws at most 300 items.

## Concepts

`concepts/` holds the interactive concept sheets the app grew out of: `floor-concepts.html` (stacked isometric floors) and `floor-concepts-02.html` (floors as columns, sorting, layouts and camera options).
