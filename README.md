# QED.bz

Personal URL Shortener based on Jekyll.

## How to Use

1. Create a new markdown file in the `_redirects` directory with the name you want for your short URL
   - For example, create `_redirects/gh.md` for the short URL `https://qed.bz/gh`
2. Add the following frontmatter:
   ```markdown
   ---
   redirect_url: https://your-destination-url.com
   ---
   ```
3. Build the site with `jekyll build`
4. The shortened URL will be available at `https://qed.bz/your-filename`

## Development

To run the site locally:

```bash
bundle install
bundle exec jekyll serve
```

## License

See the [LICENSE](LICENSE) file for details.
