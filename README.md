# rclone personal OAuth client home page

Minimal public home page and privacy policy for a **personal Google OAuth client**
used with rclone. This is not the official rclone website and is not affiliated
with the rclone project.

## URLs

| Page | URL |
| --- | --- |
| Home page | <https://minhduc0711.github.io/rclone/> |
| Privacy Policy | <https://minhduc0711.github.io/rclone/privacy/> |

The repository root redirects to `/rclone/`, and `/privacy/` redirects to
`/rclone/privacy/`.

## Google Cloud OAuth consent screen

| Field | Value |
| --- | --- |
| App name | `rclone` |
| App home page | `https://minhduc0711.github.io/rclone/` |
| App privacy policy link | `https://minhduc0711.github.io/rclone/privacy/` |
| Authorized domain | `minhduc0711.github.io` |

The app name must match the name shown on the home page. If you rename the OAuth
app, update the page to use the same name.

## Ownership verification

Google requires the home page URL to be verified in
[Google Search Console](https://search.google.com/search-console):

1. Add a URL-prefix property for `https://minhduc0711.github.io/rclone/`.
2. Choose **HTML tag** verification.
3. Put the verification meta tag into `rclone/index.html`, replacing the
   commented placeholder near the top.
4. Push, deploy, and click **Verify** in Search Console.
5. Wait at least 24 hours before retrying OAuth verification.

Alternatively, verify the root property `https://minhduc0711.github.io/` and put
the meta tag in the root `index.html`.

## Files

- `rclone/index.html` — home page
- `rclone/privacy/index.html` — privacy policy
- `rclone/assets/styles.css` — styling
- `index.html` and `privacy/index.html` — redirects for the old root URLs
- `robots.txt`, `sitemap.xml`, `.nojekyll`

## Local preview

```bash
python3 -m http.server 8000
# http://localhost:8000/rclone/
# http://localhost:8000/rclone/privacy/
```
