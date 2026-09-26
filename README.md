# Hyeongseob Jo

Hyeongseob Jo's personal blog, featuring my profile, projects, and interests.

- Website: https://johyeongseob.github.io/
- Languages: Korean and English
- Built with Jekyll and hosted on GitHub Pages

## Local Preview

Open Docker Desktop before starting the local preview, and wait until its Linux engine is running. Keep Docker Desktop running while previewing the site.

Confirm that Docker is ready:

```powershell
docker info
```

If you see a connection error mentioning `dockerDesktopLinuxEngine`, make sure Docker Desktop is open and its engine has finished starting.

Once `docker info` displays server information without a connection error, run the following command from the repository directory:

```powershell
docker compose run --rm -p 4000:4000 -p 35729:35729 jekyll sh -c "bundle install && bundle exec jekyll serve --host 0.0.0.0 --force_polling --livereload"
```

Open [http://localhost:4000](http://localhost:4000). Saving changes triggers a rebuild and automatically refreshes the browser.

- The first run may take a few minutes to install dependencies.
- After changing `_config.yml`, stop the server with `Ctrl+C` and run the command again.

## Key Files

- `_config.yml`: Profile, site settings, and navigation
- `about.md`: About page
- `_posts/`: Blog posts
- `assets/`: Images and static files
- `_includes/`, `_layouts/`, `_sass/`: Page components, layouts, and styles

## Theme and License

Based on the [Indigo theme by Sérgio Kopplin](https://github.com/sergiokopplin/indigo).

Original theme: [MIT](https://kopplin.mit-license.org/) License © Sérgio Kopplin
