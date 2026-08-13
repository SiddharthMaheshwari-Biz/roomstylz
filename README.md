# RoomStylz — Production Website

## Included
- `index.html` — responsive public website
- `thanks.html` — real Netlify Forms success destination
- `robots.txt` — allows search crawlers and points to sitemap
- `sitemap.xml` — current canonical homepage
- `roomstylz-mark.png` — supplied RoomStylz logo used as favicon/brand asset
- `roomstylz-mark-transparent.png` — supplied logo with background removed for UI use
- `apple-touch-icon.png`
- `og-image.png` — branded social/search preview poster using the supplied logo
- `site.webmanifest`
- `_headers`
- `404.html`

## Deploy
Upload/commit every file at the ROOT of the `Roomstylz` GitHub repository. Netlify should redeploy automatically.

## Form
The room-problem form uses Netlify Forms. In Netlify:
1. Open the project.
2. Open Forms and make sure form detection is enabled.
3. Submit a test form after deployment.
4. Configure an email notification under Project configuration → Notifications → Emails and webhooks → Form submission notifications.

The form submits to `thanks.html` and is not dependent on a third-party backend.

## Search indexing
After deployment:
1. Verify `https://roomstylz.netlify.app/` in Google Search Console.
2. Submit `sitemap.xml`.
3. Use URL Inspection → Request indexing for the homepage.

The site is configured with index/follow directives, canonical URL, structured data, Open Graph metadata, robots.txt and sitemap.xml.

## Before moving to a custom domain
When a permanent RoomStylz domain is purchased, update:
- canonical URL in `index.html`
- Open Graph / Twitter URLs
- JSON-LD URLs
- `robots.txt` sitemap URL
- `sitemap.xml`
- any absolute asset URLs

Then add the custom domain to the same Netlify project and set appropriate redirects.
