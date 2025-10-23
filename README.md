# Jekyll Portfolio Starter (GitHub Pages)

Minimal starter for a simple multi-page portfolio using the built-in **Cayman** theme.

## Quick Publish (no local setup)
1. Create a new repo named **your-username.github.io** (user site) _or_ any name (project site).
2. Upload these files to the repo root.
3. Commit and push. GitHub Pages will auto-publish.
   - For a **user site**, your site will be at `https://your-username.github.io`.
   - For a **project site**, enable it in: **Settings → Pages → Build and deployment → Deploy from branch → `main` / root**. Your site will be at `https://your-username.github.io/repo-name`.
4. Edit `_config.yml` and the `.md` pages to personalize.

## Optional: Custom domain
1. Add a `CNAME` file with your domain (e.g., `example.com`).
2. In your DNS, create:
   - `ALIAS`/`A`/`ANAME` to GitHub Pages apex: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` → `your-username.github.io`
3. In **Settings → Pages**, set the custom domain and enable **Enforce HTTPS**.

## Optional: Local preview
- Install Ruby and Jekyll (macOS example):
    ```bash
    brew install chruby ruby-install
    ruby-install ruby
    echo 'source /opt/homebrew/opt/chruby/share/chruby/chruby.sh' >> ~/.zshrc
    echo 'chruby ruby-3.3.0' >> ~/.zshrc
    gem install jekyll bundler
    ```
- Serve:
    ```bash
    bundle init
    echo 'gem "github-pages", group: :jekyll_plugins' >> Gemfile
    bundle install
    bundle exec jekyll serve
    ```

## Notes
- Uses the built-in `jekyll-theme-cayman` so no plugins are required.
- Add posts under `_posts/` if you want a blog: `YYYY-MM-DD-title.md` with front matter.
