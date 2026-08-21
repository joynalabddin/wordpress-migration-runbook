# WordPress Migration Runbook

A practical runbook for moving a WordPress website between hosts, domains, or environments with a clear backup, testing, and rollback process.

> **Maintainer:** Joynal Abdin · [DevJoynal](https://devjoynal.com)

## Migration principle

A migration is successful when the agreed website, data, URLs, integrations, and visitor journeys work in the new environment—not merely when the files have been copied. Plan the move around the website’s risk, traffic, database activity, email, DNS, and rollback needs.

## Choose the migration type

| Migration type | Main risk |
| --- | --- |
| Host-to-host | Configuration, PHP, database, email, and DNS differences |
| Domain change | Redirects, canonical URLs, search indexing, cookies, and mixed content |
| Staging-to-production | Incomplete content, environment URLs, credentials, and cache behavior |
| Subdirectory-to-root | Path changes, links, media URLs, and rewrite rules |
| Rebuild on new theme | Content mapping, functionality gaps, forms, and design regressions |

## Pre-migration inventory

Record the current domain and protocol, hosting details, WordPress and PHP versions, database size, media library, active theme, plugins, cron jobs, forms, email delivery, payment systems, analytics, search tools, CDN, DNS records, SSL, redirects, robots rules, XML sitemap, and important URLs.

Create a URL list for the homepage, service pages, articles, products, category pages, media files, feeds, and any page receiving traffic or backlinks. This list becomes the basis for post-migration checks and redirect decisions.

## Step-by-step runbook

### 1. Confirm access and ownership

Confirm access to the current host, new host, database, domain registrar, DNS provider, email provider, SSL controls, and relevant third-party services. Use named accounts and secure credential handling. Do not put passwords in migration notes or repository issues.

### 2. Create and verify backups

Back up the database and files separately, including uploads, configuration notes, custom code, and server-level rules where appropriate. Store a copy outside the source account and verify that the backup is readable. For a high-risk move, perform a restoration rehearsal before the live cutover.

### 3. Prepare the destination

Match or improve the required PHP version, database engine, web server behavior, storage, permissions, SSL, email configuration, and caching environment. Keep the destination private or protected while testing. Use a temporary host or local hosts-file mapping when appropriate.

### 4. Copy files and database

Transfer the WordPress files and import the database through a controlled process. Update configuration values for the destination environment. If URLs change, use a safe serialized-data-aware search-and-replace method; do not run a blind text replacement that can corrupt serialized values.

### 5. Test before DNS change

Check the login, homepage, navigation, forms, media, search, comments if used, ecommerce or payment flows, emails, scheduled tasks, redirects, 404 pages, robots rules, sitemap, analytics, SSL, mixed content, mobile layout, and important service pages. Compare key URLs against the inventory.

### 6. Plan the cutover

Lower DNS TTL ahead of a planned move where appropriate, communicate a maintenance window, pause or account for content changes during the final sync, and prepare a named rollback decision. Do not change DNS until the destination has passed the agreed tests.

### 7. Change DNS and monitor

Update the required DNS records, confirm propagation, and monitor the old and new environments. Check logs, forms, email delivery, uptime, redirects, analytics, and search-console signals. Keep the old site available but protected until the migration is confirmed.

## Post-migration checklist

- Important URLs return the intended status and content.
- HTTPS works consistently without mixed-content warnings.
- Forms, emails, payments, and external integrations work.
- Redirects exist for URLs that changed.
- The XML sitemap and robots directives are intentional.
- Cache, CDN, image delivery, and scheduled tasks behave correctly.
- Backups run in the new environment and a restore path is documented.
- Temporary access and old credentials are removed or rotated.
- The client receives a short handover note and any known limitations.

## Rollback signals

Consider rollback or a controlled maintenance state when key data is missing, payments or lead forms fail, widespread redirects are wrong, the new environment corrupts content, email is unavailable, or the team cannot restore the website safely. A rollback plan should name the decision-maker and the exact restore steps before the migration begins.

## Need WordPress migration help?

DevJoynal provides practical WordPress migration, backup, troubleshooting, and launch support.

**Explore services:** [devjoynal.com](https://devjoynal.com)

## References

- [WordPress Migration Guide](https://developer.wordpress.org/advanced-administration/upgrade/migrating/)
- [Google Search Central: Site Moves](https://developers.google.com/search/docs/crawling-indexing/site-move-with-url-changes)
- [WordPress Permalinks](https://wordpress.org/documentation/article/settings-permalinks-screen/)

## License

This runbook is for educational and operational planning purposes. A migration should be adapted to the website’s hosting, data, integrations, traffic, and rollback requirements.
