# Hugo-Website-2025 Repo

- Repo for my github.io website
- Place to make edits, check them, before pushing the site into `peterkinget.github.io` 

## Editing

1. Make edits  in this repo. You can check them live, locally with `hugo server -D`

2. Push edits to GitHub

```
> hugo server → to see the changes; close before building
> hugo build → builds into docs (see config.yml)
> git add . 
> git commit -m 'commit-message'
> git push 
```
3. Check edits on https://peterkinget.github.io/hugo-website. It might take a few minutes before the update happens.

## Publishing on peterkinget.github.io

1. Go back to `hugo-website-2025` repo

2. Rebuild the site:
```
> hugo build --baseURL "https://peterkinget.github.io/"
```
3. Push to `peterkinget.github.io` repo

```
> cd  ../peterkinget.github.io/
> \rm -rf *
> mv ../hugo-website-2025/docs/* .
> git add . 
> git commit
> git push
```
