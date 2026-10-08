# Changelog

## 1.1.1 — 2026-10-08

Hardening, large-site performance, and Joomla 7 API readiness after the 1.1.0
quality audits. Single public patch — no intermediate private releases.

### Fixed
- Stale recovery for all job modes (archive 120s, other 600s)
- Atomic `claimJob` to close the queued→running race
- `robots.txt` updates are non-fatal and compare-before-write
- Single-rename publish path (no `.previous` gap)
- Google News SQL 2-day date window (no PHP-only filter gap)
- Unicode SEF locs percent-encoded before URL validation
- Provider mappings no longer force `enabled=1` on every boot
- Install/update no longer force-re-enables disabled providers or plugins
- Tools/Dashboard no longer run expensive `#__content` probes on page load
- Recent/Current URL stats count video/business/events (not only `live`)

### Changed
- Runtime `.tmp/.htaccess` uses `IfModule` for Apache 2.4 / legacy
- Articles `Route::link` uses `xhtml=false`
- Removed unused `emitJsonAndContinue` helper
- `Factory::getLanguage()` → `$app->getLanguage()`
- Provider discovery via dispatcher + `GenericEvent` (no `triggerEvent`)
- Packaged `media/joomla.asset.json`; admin CSS stays on `addStyleSheet`
- Progress writes throttled to ~2s; `archive-progress.json` only for archive builds
- Auto retention prune (≤1/day, chunked) after successful Recent / Google News builds
- i18n for robots Options field and maintenance controller messages
- Articles/Video date windows use sargable OR predicates
- Archive month probes use index-friendly `hasContent()` LIMIT 1 lookups
- `archiveProgress` reconciles only when idle and caches status snapshots (~8s)
- Video provider mapping defaults to disabled on first insert

### Notes
- Requires Joomla 6.0+ and PHP 8.3.0+
- Install/update only through `pkg_devartsitemaps`
- For production CLI/scheduler builds, set Options `sitemap_base_url` or Joomla
  `live_site`

## 1.1.0 — 2026-08-25

Public minor release after baseline `1.0.1`. Intermediate local builds
(`1.0.2`–`1.0.14`) are not published separately.

### Added
- Fifteen packaged language packs (`en-GB`, `el-GR`, `fr-FR`, `de-DE`,
  `es-ES`, `it-IT`, `pt-PT`, `cs-CZ`, `nl-NL`, `pl-PL`, `ru-RU`, `uk-UA`,
  `ja-JP`, `tr-TR`, `zh-CN`)
- `SiteUrlResolver` for canonical sitemap base URLs
- XmlGenerator rejection of overlong/invalid loc URLs
- Schema update markers for `1.0.x` and `1.1.0`
- Argos language generation and Google gap-fill maintenance scripts

### Changed
- Administrator Dashboard Exts-style hub cards and DevArt red active submenu
- Articles `loadAlternates()` public access/category/publish filters
- Business/Events/Video absolute URLs via `SiteUrlResolver`
- Google News 2-day window compared in UTC
- Package-only GitHub updateserver
- JED/JAMSS quieting for concurrent-build guard and control-character checks

### Security
- `.tmp` directories receive `.htaccess` + `web.config` deny rules
- Invalid sitemap locs are skipped without failing the full build

### Notes
- Requires Joomla 6.0+ and PHP 8.3.0+
- Install/update only through `pkg_devartsitemaps`
- Production CLI/scheduler builds should set Options `sitemap_base_url` or
  Joomla `live_site`

## 1.0.1 — 2026-07-22

Production stability and Google Search Console compatibility.

- Root `sitemap.xml` publishes only final sitemap files
- Nested sitemap indexes are skipped from the root sitemap with logging
- Dashboard links for Main Sitemap and Google News Sitemap
- robots.txt block publishes Main + Google News sitemaps
- Cloudflare recommendation: URI Path contains `sitemaps`

## 1.0.0 — 2026-07-22

Initial public stable release for Joomla 6.

- Static XML sitemap generation outside frontend rendering
- Providers: Articles, Business, Events, Video
- Google News sitemap, archive monthly splitting, Scheduled Tasks
- Dashboard, build history, activity logs, rebuild/continue/stop/clear
