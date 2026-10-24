# Cleanup record

Source: uploaded repository ZIP, commit `ce0504d127c6c6f12a9b187daa4a6d312eb79fc0`.
This supersedes the earlier cleanup. The updated research page, including two new Work in Progress abstracts, is preserved exactly as uploaded.

## Preserved without changes

- All four main pages: Home (/home, with the existing root redirect), Research (/research), Teaching (/teaching), CV (/cv).
- Navigation, abstract styling, theme code, profile photograph, social preview image, uploaded CV, license and footer attribution.
- GitHub Actions deployment workflow, Gemfile, Dockerfile, docker-compose.yaml, _config_docker.yml, .devcontainer/devcontainer.json.
- Current domain settings and all publication text/abstracts.

## Changes

- Removed sample collections, demo/archive pages, example downloads/images, talk-map/generator tools, sample comments, and template-maintenance workflows.
- Simplified the sitemap to the four main pages.
- Added this guide, editing instructions, an optional VS Code workspace, and local preview URL overrides.
- Added Jekyll cache ignores and excluded local helper files from the published site.
- Left the author.github value `academicpages` unchanged; it is an existing template account link you may wish to replace later.

## Validation

Main page/content checksums and deployment/container/theme checksums were checked against the uploaded ZIP. Configuration parsing, literal include references, whitespace, and ZIP integrity were checked. A complete Jekyll build and Docker preview could not be run because Ruby and Docker are unavailable in this environment.

## Removed files (102)

- `.github/CONTRIBUTING.md`
- `.github/ISSUE_TEMPLATE/bug_report.md`
- `.github/ISSUE_TEMPLATE/config.yml`
- `.github/ISSUE_TEMPLATE/feature_request.md`
- `.github/PULL_REQUEST_TEMPLATE.md`
- `.github/workflows/bad-pr.yml`
- `.github/workflows/jekyll-build.yml`
- `.github/workflows/scrape_talks.yml`
- `_data/comments/layout-comments/comment-1470944006665.yml`
- `_data/comments/layout-comments/comment-1470944162041.yml`
- `_data/comments/markup-syntax-highlighting/comment-1470969665387.yml`
- `_data/comments/welcome-to-jekyll/comment-1470942205700.yml`
- `_data/comments/welcome-to-jekyll/comment-1470942247755.yml`
- `_data/comments/welcome-to-jekyll/comment-1470942265819.yml`
- `_data/comments/welcome-to-jekyll/comment-1470942493518.yml`
- `_drafts/post-draft.md`
- `_pages/archive-layout-with-content.md`
- `_pages/category-archive.html`
- `_pages/collection-archive.html`
- `_pages/markdown.md`
- `_pages/non-menu-page.md`
- `_pages/page-archive.html`
- `_pages/portfolio.html`
- `_pages/publications.html`
- `_pages/tag-archive.html`
- `_pages/talkmap.html`
- `_pages/talks.html`
- `_pages/terms.md`
- `_pages/year-archive.html`
- `_portfolio/portfolio-1.md`
- `_portfolio/portfolio-2.html`
- `_posts/2012-08-14-blog-post-1.md`
- `_posts/2013-08-14-blog-post-2.md`
- `_posts/2014-08-14-blog-post-3.md`
- `_posts/2015-08-14-blog-post-4.md`
- `_posts/2199-01-01-future-post.md`
- `_publications/2009-10-01-paper-title-number-1.md`
- `_publications/2010-10-01-paper-title-number-2.md`
- `_publications/2015-10-01-paper-title-number-3.md`
- `_publications/2024-02-17-paper-title-number-4.md`
- `_publications/2025-06-08-paper-title-number-5.md`
- `_talks/2012-03-01-talk-1.md`
- `_talks/2013-03-01-tutorial-1.md`
- `_talks/2014-02-01-talk-2.md`
- `_talks/2014-03-01-talk-3.md`
- `_teaching/2014-spring-teaching-1.md`
- `_teaching/2015-spring-teaching-2.md`
- `files/bibtex1.bib`
- `files/paper1.pdf`
- `files/paper2.pdf`
- `files/paper3.pdf`
- `files/slides1.pdf`
- `files/slides2.pdf`
- `files/slides3.pdf`
- `images/500x300.png`
- `images/apple-touch-icon-180x180.png`
- `images/bio-photo-2.jpg`
- `images/bio-photo.jpg`
- `images/editing-talk.png`
- `images/favicon-192x192.png`
- `images/favicon-32x32.png`
- `images/favicon-512x512.png`
- `images/favicon.ico`
- `images/favicon.svg`
- `images/manifest.json`
- `images/profile.png`
- `images/themes/homepage-air-dark.png`
- `images/themes/homepage-air-light.png`
- `images/themes/homepage-contrast-dark.png`
- `images/themes/homepage-contrast-light.png`
- `images/themes/homepage-dark.png`
- `images/themes/homepage-dirt-dark.png`
- `images/themes/homepage-dirt-light.png`
- `images/themes/homepage-light.png`
- `images/themes/homepage-mint-dark.png`
- `images/themes/homepage-mint-light.png`
- `images/themes/homepage-sunrise-dark.png`
- `images/themes/homepage-sunrise-light.png`
- `images/wiki/plotly_example.png`
- `markdown_generator/OrcidToBib.ipynb`
- `markdown_generator/PubsFromBib.ipynb`
- `markdown_generator/README.md`
- `markdown_generator/publications.csv`
- `markdown_generator/publications.ipynb`
- `markdown_generator/publications.py`
- `markdown_generator/publications.tsv`
- `markdown_generator/pubsFromBib.py`
- `markdown_generator/talks.ipynb`
- `markdown_generator/talks.py`
- `markdown_generator/talks.tsv`
- `scripts/README.md`
- `scripts/make-og-image.py`
- `talkmap.ipynb`
- `talkmap.py`
- `talkmap/leaflet_dist/MarkerCluster.Default.css`
- `talkmap/leaflet_dist/MarkerCluster.css`
- `talkmap/leaflet_dist/leaflet.markercluster-src.js`
- `talkmap/leaflet_dist/leaflet.markercluster.js`
- `talkmap/leaflet_dist/screen.css`
- `talkmap/map.html`
- `talkmap/org-locations.js`
- `talkmap_out.ipynb`
