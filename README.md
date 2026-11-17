# Important commands

- Run locally: `bundle exec jekyll serve --livereload`
- Add: `git add --all`
- Commit: `git commit -m "message"`
- Push: `git push -u origin main`
- Force (if needed): `git push -u origin main --force`

# TODO

- Style theme toggle button
- Merge theme stylesheets and move variables into classes for html block
- Look into minima for markdown support. Implement for posts.
	- Bold and headers working.
	- Links working
	- Images working
	- HTML working
	- Code (inline and block) not working.

# Ideas

- Add a post field that highlights them gold and places them at the top of the homepage.

# Other notes

- Writers will publish markdown file/article text through Github Issues.

## Development and layout

Install the Ruby dependencies with `bundle install`, then run `bundle exec jekyll serve`; validate with `bundle exec jekyll build`. `_posts/` contains dated articles, `_layouts/` supplies page templates, and `_includes/` contains shared head, navigation, and widgets. Styles live in `assets/css/`; the favicon remains under `assets/`. Keep URLs wrapped in Liquid's `relative_url` filter when used by templates so configured base paths work.

Theme switching must use the light/dark stylesheets in `assets/css/`. Generated `_site/` output is not source content.
