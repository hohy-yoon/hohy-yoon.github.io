# Hohyun Yoon's website

This is a cleaned copy of hohy-yoon/hohy-yoon.github.io based on commit ce0504d.
The ZIP includes Git history. Cleanup changes are uncommitted on master so you can review them in VS Code before publishing.

## Everyday editing

| Edit | File |
| --- | --- |
| Homepage | `_pages/about.md` |
| Research and abstracts | `_pages/research.md` |
| Teaching | `_pages/teaching.html` |
| CV link | `_pages/cv.md` |
| Menu | `_data/navigation.yml` |
| Name, contact details, domain | `_config.yml` |
| Abstract spacing and browser-tab icon | `_includes/head/custom.html` |
| Profile photograph | `images/ProfilePhoto.jpg` |
| Uploaded CV | `files/YoonCV.pdf` |

The CV page currently links to Google Drive. Updating files/YoonCV.pdf alone will not change that destination.

## Open and preview in VS Code

1. Extract the ZIP to a permanent folder. Open the extracted `hohy-yoon.github.io` folder in VS Code.
2. Install and start Docker Desktop. Install Microsoft's Dev Containers extension in VS Code.
3. Press Command-Shift-P and select **Dev Containers: Reopen in Container**.
4. Allow the first container build to finish. Open http://localhost:4000/home.
5. If preview has not started, open a terminal inside the container and run:

```bash
bundle exec jekyll serve --host 0.0.0.0 --port 4000 --watch --config _config.yml,_config_docker.yml
```

Leave that terminal running. If the port is already in use, a preview server may already be running. Save edits and refresh your browser. Restart the server after changing _config.yml. The original container setup is preserved; it has not been run or verified in the cleanup environment.

If Ruby and Bundler are already installed locally, an alternative is:

```bash
bundle install
bundle exec jekyll serve --config _config.yml,_config_local.yml --host localhost --port 4000
```

The optional HohyunYoon.code-workspace file hides theme internals from the Explorer. It does not delete them. Opening the project folder normally shows all folders.

## Review, commit, and publish

1. In VS Code, open Source Control. Review the deletions and changed files listed in CLEANUP.md.
2. Confirm the branch is master. Stage the changes and commit with a message such as `Remove unused template content`.
3. Push (or Sync Changes) and sign in to GitHub if prompted. GitHub Desktop is not required.
4. Watch the deployment in the repository's Actions tab. A successful deployment publishes the changes.

Saving files and committing locally do not publish them; pushing master triggers deployment. If GitHub has newer commits, pull and resolve any differences before pushing; do not force push.

Your production URL remains https://www.hohyunyoon.com. This cleanup does not change DNS or certificate settings.

## Theme files

Keep _includes, _layouts, _sass, assets, Gemfile, LICENSE, and the deployment/container files. These power the site even though most are not edited regularly. The theme's original license and attribution are retained.
