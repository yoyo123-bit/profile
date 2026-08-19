# Profile site

This is a simple static profile page. To publish it on GitHub Pages using the included GitHub Actions workflow, create a GitHub repository and push the `main` branch. The workflow will build and deploy the repository contents to the `gh-pages` branch.

Quick commands to create a repo (using the GitHub CLI `gh`):

```bash
# create a repository on GitHub and push the local repo
gh repo create MY-USERNAME/MY-REPO --public --source=. --remote=origin --push
```

If you prefer to create the repo on GitHub.com, add the remote and push manually:

```bash
git remote add origin https://github.com/<your-username>/<repo>.git
git branch -M main
git push -u origin main
```

After pushing, GitHub Actions will run and deploy to GitHub Pages. Visit `https://<your-username>.github.io/<repo>/` once the Action completes.
