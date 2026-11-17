# Marcelo Guzmán — researcher profile

Minimal static website for <https://maguzj.github.io/>. The page content and styles are in `index.html`; no build or dependencies are required.

## Edit and preview locally

Edit `index.html` in a text editor. From the folder containing that file, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://127.0.0.1:8000/> and refresh after saving changes. Stop the server with Ctrl+C.

## Connect to the existing GitHub repository

This source folder was initially created without Git history. To work with the existing published repository, clone it into a new sibling folder and copy the updated page into that checkout:

```sh
cd /Users/marceloguzmanjara
git clone https://github.com/maguzj/maguzj.github.io.git maguzj.github.io
cp /Users/marceloguzmanjara/webpage/index.html /Users/marceloguzmanjara/maguzj.github.io/index.html
cd /Users/marceloguzmanjara/maguzj.github.io
git diff -- index.html
```

Use that cloned folder for future edits. If it already exists as a checkout, use it instead of cloning again.

After reviewing and previewing changes, publish from the checkout:

```sh
git add index.html
git commit -m "Update researcher profile"
git push
```

GitHub Pages publishes from the branch and folder selected in the repository's Pages settings. The intended configuration is `main` and `/(root)`.

## Content sources and remaining work

- Current role and background: [QBio profile](https://qbio.ens.psl.eu/en/people/marcelo-guzman).
- Research directions: [QBio interview](https://qbio.ens.psl.eu/en/newsroom/marcelo-guzman-junior-research-chair-fellow-qbio).
- Professional email: [LPENS directory entry](https://www.lpens.ens.psl.eu/laboratory/directory/?id=1988&lang=en).
- Publication list: [Google Scholar](https://scholar.google.com/citations?user=ktPeQ3MAAAAJ&hl=en). The site links to the profile rather than duplicating a list that needs manual updates.
- A CV is not available yet, so the page omits it. Add a link when the current CV is ready.

Role, research directions, and email were checked on 17 November 2026. No claims of completed results were inferred from the research plans in the interview.
