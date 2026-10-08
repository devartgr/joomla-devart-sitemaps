# DevArt Sitemaps

DevArt Sitemaps is a Joomla 6 package for generating static XML sitemap files
outside normal frontend rendering.

## Requirements

- Joomla 6.0+
- PHP 8.3.0+

## Package

Current public version: **`1.1.1`**

Contains:

- Component `com_devartsitemaps`
- Provider plugin `plg_devartsitemap_devartarticles`
- Provider plugin `plg_devartsitemap_devartbusiness`
- Provider plugin `plg_devartsitemap_devartevents`
- Provider plugin `plg_devartsitemap_devartvideo`
- Scheduler plugin `plg_task_devartsitemaps`

The package provides an administrator dashboard, provider discovery,
batch-based recent and archive sitemap generation, a dedicated Google News
sitemap, provider-specific clear and rebuild flows, Joomla Scheduled Tasks
integration, static sitemap file output, and a root sitemap that references
final sitemap files directly. Provider plugins remain independently
discoverable through the `devartsitemap` plugin group.

Fifteen administrator language packs are included (`en-GB`, `el-GR`, `fr-FR`,
`de-DE`, `es-ES`, `it-IT`, `pt-PT`, `cs-CZ`, `nl-NL`, `pl-PL`, `ru-RU`,
`uk-UA`, `ja-JP`, `tr-TR`, `zh-CN`).

Install and update only through `pkg_devartsitemaps`. Updates are served from
the GitHub package updateserver.

For production CLI or Scheduled Task builds, set Options
`Public sitemap base URL` (`sitemap_base_url`) or Joomla `live_site` so
generated locs do not depend on a request-derived host.

## Development

`source/` is the only development source. Generated packages belong under
`builds/`. Public release ZIPs are copied under `releases/`.

Validate and build with:

```shell
php scripts/validate.php
php scripts/build.php
```

The build script follows `source/package/pkg_*.xml`, creates only the inner ZIPs
declared by that manifest, and writes an outer package plus its SHA-256 file.

## Verification

Repository validation and package generation do not constitute Joomla runtime
verification. Complete local Herd smoke QA and VPS Joomla QA before recording a
version as verified in `PROJECT_STATUS.md`.
