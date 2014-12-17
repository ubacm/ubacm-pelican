ubacm-pelican
=============

UB ACM Pelican build with content and pages.

Description
===========
This repo contains the raw files for building the UB ACM website. When modifying, we are primarily concerned with `content` and `theme`.

`content` consists of Markdown files (with some HTML for hacks) that Pelican uses to render pages. When adding new pages (or blog posts when we support that), add that here.

`theme` is a modification of the Bootstrap Jumbotron example page. Any changes to the actual site templating live here.

Building and Running
====================
First time:

1. Clone the repo down.
2. Create a virtualenv for the project: `virtualenv --distribute env`.
3. Start the virtualenv: `source env/bin/active`.
4. Add the dependencies: `pip install -R requirements.txt`.

Actually building and running: 
1. `fab reserve`, which is a combination of `fab build` and `fab serve`.
