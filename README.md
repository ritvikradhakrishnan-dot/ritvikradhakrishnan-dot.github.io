# Ritvik Ramanan Radhakrishnan — personal website

A static academic homepage with an introduction, research papers, and talks.
It uses plain HTML and CSS, with no build step or dependencies.

## Files

- `index.html` — biography, publications, author names, and links to articles and talks.
- `style.css` — colours, typography, spacing, and mobile layout.

Keep both files in the same folder so the page can load its stylesheet.

## Preview

Open `index.html` in a browser. After editing either file, save it and refresh
the page. Check both a wide window and a narrow window to review the mobile layout.

Alternatively, run this command from the `website` folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8000>. Press `Ctrl+C` in the terminal to stop the server.

## Editing

Update the text and links in `index.html`. To add a paper or talk, copy an
existing `<li class="entry">` within the relevant section and replace its contents.
Use full coauthor names and update both the displayed date and the `datetime`
attribute when adding a talk.

The colour and page-width settings are at the top of `style.css`. Mobile styles
are in the `@media (max-width: 560px)` block.

## Publishing

This folder is a local working copy. Changes here do not automatically update
the GitHub repository or the live website.

Copy the updated `index.html` and `style.css` into the root of the website
repository at `/Users/rradhakrishn/Documents/GitHub/ritvikrr.github.io`, review
the changes, and commit and push them through the repository's usual publishing
workflow. Keep this working copy and the repository copy in sync.
