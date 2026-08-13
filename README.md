# RoomStylz — Production Website

This package is the cleaned production build for the RoomStylz public website.

## Important fixes in this build
- Uses the supplied RoomStylz preview poster as `og-image.png`.
- Header wordmark is rendered as **RoomStylz** with no accidental space.
- Removed the visible “Skip to content” element.
- Rebuilt the footer with proper columns, spacing, lists and mobile stacking.
- Replaced the old circular “RoomStylz Tested” stamp with a cleaner certification card using the real RoomStylz mark.
- Form submission is handled as a real Netlify Form POST and redirects to `thanks.html` only after a successful submission.
- Kept SEO basics: canonical, robots, sitemap, structured data and social metadata.
- Kept favicon, Apple touch icon and web manifest.

## Deploy
Commit/upload every file at the ROOT of the `Roomstylz` GitHub repository. If the repository is connected to Netlify, the new commit should deploy automatically.

## Netlify Form
After deployment:
1. Open the Netlify project.
2. Go to **Forms** and confirm `room-problem` is detected.
3. Submit a real test from the website.
4. Confirm the submission appears in Netlify Forms.
5. Configure email notifications if desired.

The browser submits to the site root through Netlify Forms and then redirects to `/thanks.html`. This avoids relying on a direct POST to an HTML success page.

## SEO
After deployment, verify the site in Google Search Console and submit:
`https://roomstylz.netlify.app/sitemap.xml`

The site is prepared for indexing, but search indexing/ranking is not guaranteed.

## Custom domain later
When a permanent RoomStylz domain is added, update the canonical URL, Open Graph URLs, JSON-LD URLs, sitemap and robots sitemap URL.
