# Blogger / Blogspot to WordPress Migration Runbook

A practical, SEO-conscious runbook for moving a Blogger or Blogspot website to WordPress while protecting content quality, media, URLs, and the visitor experience.

> **Maintainer:** Joynal Abdin · [DevJoynal](https://devjoynal.com)

## What Blogger-to-WordPress Migration Involves

A Blogger migration is more than exporting text. A careful transfer includes the WordPress destination, posts, pages, images, embedded media, labels, dates, authors, comments where supported, URL structure, internal links, redirects, search visibility, and post-migration testing.

The exact result depends on the Blogger template, custom widgets, media sources, comment system, HTML structure, and target WordPress setup. This runbook favors a transparent scope and quality checks over promising a perfect one-click transfer for every site.

## Pre-Migration Checklist

### 1. Audit the Blogger site

- Record the current custom domain, Blogspot address, HTTPS status, and approximate post/page count.
- Review the URL pattern, labels, authors, dates, comments, images, videos, downloads, and embedded content.
- List important landing pages, high-traffic posts, subscription forms, custom widgets, and external integrations.
- Crawl or export a URL inventory so important pages can be checked after launch.

### 2. Back up the source

- Download the Blogger export XML file from **Settings → Manage blog → Back up content**.
- Save a copy of important images, downloadable files, theme assets, and any custom HTML.
- Keep the original Blogger site available until the WordPress version and redirects have been validated.
- Preserve a dated copy of the URL inventory and migration notes.

### 3. Prepare WordPress

- Set up hosting, HTTPS, the production domain or a protected staging site, and a current WordPress version.
- Configure permalinks deliberately rather than accepting a structure that conflicts with the old URLs.
- Create the required users, categories, tags, menus, widgets, and essential pages.
- Install only the migration, SEO, redirect, caching, and security tools needed for the agreed scope.
- Confirm a working WordPress backup and a rollback plan before importing content.

## Content Transfer Workflow

### 1. Export and import

1. Export the Blogger XML and keep the original file unchanged.
2. Import the content into a clean WordPress staging environment using a suitable Blogger importer or an agreed manual process.
3. Review the import report and compare the expected number of posts, pages, comments, and authors with the result.
4. Do not publish a bulk import before checking formatting, metadata, and media.

### 2. Normalize content

- Map Blogger **labels** to an intentional WordPress category and tag structure; do not create hundreds of accidental duplicates.
- Preserve original publication dates and authors where possible, and document any exceptions.
- Check headings, paragraphs, lists, tables, code, shortcodes, captions, and embedded videos.
- Remove obsolete Blogger-specific markup only after confirming that the visible content still works.
- Review internal links for old Blogspot addresses, attachment URLs, and broken anchors.

### 3. Check images and media

- Confirm that featured images and inline images display correctly on the new domain.
- Check whether images still point to Blogger’s image/CDN host and decide whether they should be downloaded, re-hosted, or intentionally retained.
- Test image sizes, filenames, alt text, captions, lazy loading, and responsive behavior.
- Rebuild unsupported widgets, forms, galleries, downloads, and video embeds instead of assuming they will transfer automatically.

## URL Structure and Redirect Planning

- Compare the old Blogger URL pattern with the planned WordPress permalink structure before launch.
- Build a redirect map for the homepage, posts, pages, label archives, feeds where relevant, and other important indexed URLs.
- Use permanent redirects only when the destination is a genuine equivalent; avoid sending every old URL to the homepage.
- Check trailing slashes, date segments, URL encoding, HTTPS, canonical URLs, and host variations.
- Test redirects from both the old Blogspot address and the old custom domain when applicable.
- Update internal links, XML sitemaps, canonical tags, Search Console properties, analytics settings, and social profile links after launch.

## Post-Migration Validation Checklist

### Content and design

- [ ] Expected posts and pages are present.
- [ ] Titles, dates, authors, labels/categories, tags, excerpts, and featured images are correct.
- [ ] Images, videos, downloads, forms, menus, widgets, comments, and embeds work.
- [ ] Mobile, tablet, and desktop layouts have been reviewed.

### Technical and SEO checks

- [ ] HTTPS works consistently and mixed-content warnings are resolved.
- [ ] Important old URLs resolve through the planned redirects.
- [ ] New URLs return the correct status code and do not create redirect chains.
- [ ] Canonical URLs, robots rules, XML sitemap, pagination, and noindex settings are intentional.
- [ ] Internal links, 404 pages, search, feeds, and navigation have been tested.
- [ ] Search Console, analytics, email, forms, caching, and security monitoring are connected.

### Launch and monitoring

- [ ] A fresh WordPress backup exists immediately before launch.
- [ ] DNS and domain changes are scheduled with a rollback contact and maintenance plan.
- [ ] The old Blogger site is kept available while redirects and indexing are monitored.
- [ ] Crawl errors, traffic, rankings, server logs, and user reports are reviewed after launch.
- [ ] Any missing media, broken links, formatting issues, or redirect gaps are documented and fixed.

## Common Blogger Migration Issues

| Issue | Practical response |
| --- | --- |
| Images remain on Blogger’s CDN | Audit image URLs, re-host where appropriate, and verify every important image after import. |
| Custom widgets do not transfer | Recreate forms, navigation, subscription tools, galleries, and scripts with WordPress-compatible alternatives. |
| Comments are incomplete | Identify the source comment system, confirm what the importer supports, and plan a separate export or replacement when necessary. |
| Labels create poor taxonomy | Review labels before import and map them to a smaller, useful category/tag structure. |
| Old URLs return 404 errors | Use a tested redirect map for valuable posts and pages; do not rely on a blanket homepage redirect. |
| Formatting contains Blogger markup | Clean and review HTML in batches, then manually inspect high-value posts and unusual layouts. |
| Search visibility changes after launch | Verify canonicals, sitemap, redirects, robots rules, indexing settings, and Search Console coverage. |

## Rollback and Documentation

Keep the Blogger export, WordPress backup, URL map, import notes, redirect rules, known issues, and launch checklist together. If a serious problem appears, restore the agreed backup or return DNS to the previous environment while the issue is investigated. Record what was changed so future maintenance is repeatable.

## Need Blogger-to-WordPress Migration Help?

Need to move a Blogger or Blogspot site to WordPress? Visit [devjoynal.com](https://devjoynal.com) to discuss content transfer, media checks, URL mapping, redirects, SEO-conscious structure, and post-migration support.

You can also follow [DevJoynal on Facebook](https://web.facebook.com/DevJoynal/).

**Move the content carefully. Preserve the URLs. Launch with confidence.**
