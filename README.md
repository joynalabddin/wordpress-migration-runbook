# Blogger to WordPress Migration Runbook

[![Blogger](https://img.shields.io/badge/Source-Blogger%2FBlogspot-F57C00?style=for-the-badge&logo=blogger&logoColor=white)](https://www.blogger.com/)
[![WordPress](https://img.shields.io/badge/Destination-WordPress-21759B?style=for-the-badge&logo=wordpress&logoColor=white)](https://wordpress.org/)
[![Maintained by DevJoynal](https://img.shields.io/badge/Maintained_by-DevJoynal-111827?style=for-the-badge)](https://devjoynal.com)

A practical, SEO-conscious runbook for moving a **Blogger or Blogspot website to WordPress** while protecting content, images, authors, dates, URLs, redirects, and the visitor experience.

> **Migration is more than exporting an XML file.** A successful transfer prepares the destination, maps the content, checks media and formatting, preserves important URLs, validates the new site, and monitors the launch.

[Visit DevJoynal](https://devjoynal.com/?utm_source=github&utm_medium=referral&utm_campaign=blogger-wordpress-migration) · [WordPress Malware Removal Checklist](https://github.com/joynalabddin/wordpress-security-checklist) · [DevJoynal on Facebook](https://web.facebook.com/Devjoynal/)

## What This Runbook Covers

This guide is designed for site owners, bloggers, developers, and support teams planning a Blogger-to-WordPress migration. It covers source auditing, Blogger XML backup, WordPress preparation, content transfer, images and embedded media, labels, authors, dates, URL planning, redirects, SEO validation, launch monitoring, and rollback documentation.

Every site is different. Blogger templates, custom widgets, comments, media hosts, URL patterns, and unusual HTML may require manual review. This runbook promotes a transparent scope and quality checks rather than promising a perfect one-click migration for every website.

## Quick Migration Map

| Stage | Main outcome |
| --- | --- |
| Audit | A source inventory, risk list, and agreed migration scope |
| Backup | A preserved Blogger export and supporting source assets |
| Prepare | A secure WordPress destination with intentional permalinks |
| Transfer | Posts, pages, media, labels, authors, dates, and supported comments moved and reviewed |
| Redirect | Important old URLs mapped to genuine new destinations |
| Validate | Content, design, SEO, forms, media, and redirects tested before launch |
| Monitor | Search visibility, errors, traffic, and user reports reviewed after launch |

## Before You Start

### Audit the Blogger website

- [ ] Record the custom domain, Blogspot address, HTTPS status, language, and approximate post/page count.
- [ ] Export or crawl a URL inventory covering posts, pages, label archives, feeds where relevant, images, downloads, and important landing pages.
- [ ] Review the Blogger template, custom widgets, navigation, subscription forms, comments, videos, scripts, and third-party integrations.
- [ ] Identify high-traffic, high-conversion, frequently linked, and recently updated content.
- [ ] Confirm who owns the domain, hosting, DNS, analytics, Search Console, and social accounts.

### Define the migration scope

Decide in writing what will be transferred, rebuilt, excluded, or reviewed manually. Clarify whether the project includes the custom domain, comments, media re-hosting, taxonomy redesign, SEO metadata, redirects, design recreation, performance work, security hardening, and post-launch support.

> **Good scope prevents bad surprises.** Do not treat widgets, comments, images, unusual HTML, and URL changes as automatic parts of a basic XML import.

## Backup Checklist

- [ ] Download the Blogger export XML from **Settings → Manage blog → Back up content**.
- [ ] Keep the original XML unchanged and store a second dated copy safely.
- [ ] Save important images, downloadable files, theme assets, custom HTML, and integration settings where applicable.
- [ ] Record the existing URL inventory, analytics configuration, Search Console properties, and DNS settings.
- [ ] Keep the original Blogger site available until the WordPress version and redirects have been tested.

## Prepare the WordPress Destination

- [ ] Use a supported WordPress version, HTTPS, reliable hosting, and a protected staging environment.
- [ ] Configure the custom domain and decide whether the site will launch at the final domain or a temporary URL.
- [ ] Choose a permalink structure after comparing it with the old Blogger URLs.
- [ ] Create required users, categories, tags, menus, pages, forms, widgets, and essential integrations.
- [ ] Install only the required migration, SEO, redirect, caching, backup, and security tools.
- [ ] Confirm that backups work and that a rollback path exists before importing content.

## Content Transfer Workflow

### 1. Export and import

1. Export the Blogger XML and keep the source copy unchanged.
2. Import into a clean WordPress staging environment using a suitable Blogger importer or an agreed manual process.
3. Compare the expected number of posts, pages, comments, authors, and media references with the import result.
4. Review the import report before publishing anything in bulk.
5. Keep a list of failed, duplicated, empty, or partially imported items for manual correction.

### 2. Normalize posts and pages

- [ ] Preserve original publication dates and authors where possible, documenting exceptions.
- [ ] Review titles, headings, paragraphs, lists, tables, code, captions, excerpts, and embedded videos.
- [ ] Map Blogger **labels** to an intentional WordPress category and tag structure.
- [ ] Remove obsolete Blogger markup only after confirming that visible content and links still work.
- [ ] Check internal links for old Blogspot addresses, attachment URLs, redirects, and broken anchors.
- [ ] Review duplicate content, empty posts, drafts, scheduled posts, and unwanted imported pages.

### 3. Check images and media

- [ ] Confirm that featured images and inline images display correctly on the new domain.
- [ ] Identify images still hosted on Blogger’s image/CDN infrastructure.
- [ ] Decide whether media should be downloaded and re-hosted, intentionally retained, or replaced.
- [ ] Test image filenames, dimensions, alt text, captions, lazy loading, responsive behavior, and compression.
- [ ] Rebuild unsupported widgets, galleries, forms, downloads, scripts, and video embeds with WordPress-compatible alternatives.

## URL Structure and Redirect Planning

- [ ] Compare the old Blogger URL pattern with the proposed WordPress permalink structure before launch.
- [ ] Create a redirect map for the homepage, posts, pages, important labels, feeds where relevant, and high-value indexed URLs.
- [ ] Send each old URL to a genuine equivalent; do not send every URL to the homepage.
- [ ] Check trailing slashes, date segments, URL encoding, HTTPS, host variations, and canonical URLs.
- [ ] Test redirects from the old Blogspot address and the old custom domain when applicable.
- [ ] Avoid redirect chains, redirect loops, mixed-content warnings, and accidental noindex settings.
- [ ] Update internal links, XML sitemaps, Search Console properties, analytics, canonical tags, and social profile links.

## Pre-Launch Validation

### Content and design

- [ ] Expected posts, pages, labels/categories, tags, authors, dates, excerpts, and featured images are present.
- [ ] Images, videos, downloads, forms, menus, widgets, comments, and embeds work.
- [ ] High-value pages have been manually reviewed for formatting and missing content.
- [ ] Mobile, tablet, desktop, accessibility basics, and navigation have been tested.

### Technical and SEO checks

- [ ] HTTPS works consistently and mixed-content warnings are resolved.
- [ ] Important old URLs resolve through the planned redirects.
- [ ] New URLs return the correct status code and do not create chains or loops.
- [ ] Canonical URLs, robots rules, XML sitemap, pagination, and noindex settings are intentional.
- [ ] Internal links, 404 pages, search, feeds, structured data, and navigation have been tested.
- [ ] Search Console, analytics, email, forms, caching, backups, and security monitoring are connected.

## Launch and Monitoring

- [ ] Create a fresh WordPress backup immediately before launch.
- [ ] Schedule DNS or domain changes with a rollback contact and maintenance window.
- [ ] Keep the original Blogger site available while redirects and indexing are monitored.
- [ ] Review crawl errors, indexing coverage, traffic, server logs, uptime, and user reports after launch.
- [ ] Document missing media, broken links, formatting issues, redirect gaps, and fixes.
- [ ] Recheck high-value URLs after the first meaningful traffic and crawl period.

## Common Blogger Migration Issues

| Issue | Practical response |
| --- | --- |
| Images remain on Blogger’s CDN | Audit image URLs, re-host where appropriate, and verify every important image after import. |
| Custom widgets do not transfer | Recreate forms, navigation, subscription tools, galleries, and scripts with WordPress-compatible alternatives. |
| Comments are incomplete | Confirm what the importer supports and plan a separate export, replacement, or manual review where necessary. |
| Labels create poor taxonomy | Review labels before import and map them to a smaller, useful category/tag structure. |
| Old URLs return 404 errors | Use a tested redirect map for valuable posts and pages; do not rely on a blanket homepage redirect. |
| Formatting contains Blogger markup | Clean and review HTML in batches, then manually inspect high-value posts and unusual layouts. |
| Search visibility changes after launch | Verify canonicals, sitemap, redirects, robots rules, indexing settings, and Search Console coverage. |
| Content imports with duplicates | Compare counts, identify duplicate slugs or posts, and document the final canonical version. |

## Rollback and Documentation

Keep the Blogger export, WordPress backup, URL map, import notes, redirect rules, known issues, launch checklist, and access-owner details together. If a serious problem appears, restore the agreed backup or return DNS to the previous environment while the issue is investigated. Record what changed so future maintenance is repeatable.

## Need Blogger-to-WordPress Migration Help?

I’m **Joynal Abdin**, a Blogger/Blogspot-to-WordPress Migration Expert working through [DevJoynal](https://devjoynal.com/?utm_source=github&utm_medium=referral&utm_campaign=blogger-wordpress-migration). I help with content transfer, media checks, labels, dates, authors, URL mapping, redirects, SEO-conscious structure, and post-migration support.

> Planning to move a Blogger or Blogspot website to WordPress? Visit [devjoynal.com](https://devjoynal.com/?utm_source=github&utm_medium=referral&utm_campaign=blogger-wordpress-migration) and share the current URL, approximate content size, preferred timeline, and any migration concerns.

## Related DevJoynal Resources

- [WordPress Malware Removal Checklist](https://github.com/joynalabddin/wordpress-security-checklist)
- [WordPress Website Development Guide](https://github.com/joynalabddin/wordpress-website-development-guide)
- [WordPress Speed Optimization Checklist](https://github.com/joynalabddin/wordpress-speed-optimization-checklist)
- [WordPress SEO Checklist](https://github.com/joynalabddin/wordpress-seo-checklist)
- [DevJoynal on Facebook](https://web.facebook.com/Devjoynal/)

## Maintainer

**Joynal Abdin · DevJoynal**  
Blogger/Blogspot Migration · WordPress Development · SEO-conscious Website Transfers  
[https://devjoynal.com](https://devjoynal.com)

**Move the content carefully. Preserve the URLs. Launch with confidence.**
