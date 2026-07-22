
# DevArt Sitemaps for Joomla

Professional Joomla 6 XML sitemap solution designed for business websites, news portals, magazines, municipalities, organizations, enterprise deployments, and high-performance websites with small or very large content collections.

![Joomla](https://img.shields.io/badge/Joomla-6.x-blue)
![PHP](https://img.shields.io/badge/PHP-8.2%2B-green)
![Release](https://img.shields.io/badge/Version-1.0.1-orange)
![License](https://img.shields.io/badge/License-GPLv3-red)

---

## Overview

DevArt Sitemaps is a modern Joomla 6 native XML sitemap generator built for performance, scalability, reliability and production deployments.

Instead of generating XML dynamically on every request, DevArt Sitemaps builds optimized static XML files that can be served efficiently by Joomla, web servers and CDNs, dramatically reducing database load while providing excellent scalability for high-traffic websites.

The extension supports multiple content providers, automatic archive generation, Google News sitemaps, Joomla Scheduled Tasks, enterprise-scale sitemap management and production-safe sitemap validation.

---

## Features

### Static XML Sitemap Generation

Generate production-ready static XML sitemaps for maximum performance.

Supported providers:

- Joomla Articles
- DevArt Business
- DevArt Events
- DevArt Video

Features include:

- Static XML generation
- Automatic sitemap generation
- Provider-based architecture
- Automatic sitemap splitting
- XML validation
- Root sitemap validation
- Automatic rebuild tools
- Production-safe sitemap publishing

---

### Google News

Built-in Google News sitemap generation.

Features include:

- Google News compatible XML
- Recent news support
- Automatic updates
- XML validation
- Native Joomla integration

Ideal for editorial and news websites.

---

### Archive Engine

Designed for websites containing hundreds of thousands or millions of URLs.

Features include:

- Monthly archive generation
- Automatic archive splitting
- Continue builds
- Stop builds
- Rebuild from scratch
- Provider isolation
- Optimized large dataset processing

Suitable for long-term content archives.

---

### Scheduler Integration

Native Joomla Scheduled Tasks support.

Features include:

- Automatic sitemap generation
- Scheduled rebuilds
- Background processing
- Scheduler health monitoring
- Safe task execution

---

### Dashboard

Central management interface.

Features include:

- Main Sitemap information
- Google News Sitemap information
- Sitemap statistics
- Scheduler status
- Build history
- Activity logs
- Provider overview
- System health information
- Cloudflare recommendations

---

### Performance

Built for production environments.

Features:

- Static XML generation
- Optimized database queries
- Minimal server load
- Low memory usage
- Cloudflare friendly
- CDN friendly
- Enterprise scalability
- Large dataset support

Suitable for:

- News portals
- Business websites
- Corporate websites
- Municipal websites
- Educational institutions
- Associations
- Government websites
- Enterprise Joomla installations

---

### Joomla Native Updates

Supports Joomla native updates via GitHub.

Update Server:

https://raw.githubusercontent.com/devartgr/joomla-devart-sitemaps/main/pkg_devartsitemaps_update.xml

---

## Included Extensions

This package installs:

- com_devartsitemaps
- plg_task_devartsitemaps

---

## Requirements

- Joomla 6.x
- PHP 8.2+

---

## Security

Built-in protection includes:

- Joomla ACL
- CSRF protection
- SQL parameter binding
- Safe XML generation
- Root sitemap validation
- XML structure validation
- Server-side validation
- Secure file operations

Designed for secure production deployments.

---

## Compatibility

Supported:

- Joomla 6.x
- PHP 8.2+
- Joomla Scheduled Tasks
- Joomla Update Server
- Cloudflare
- CDN environments
- Modern Joomla MVC architecture

Not Supported:

- Joomla 3
- Joomla 4
- Joomla 5
- Legacy PHP versions

---

## Current Version

**1.0.1**

---

## What's New in 1.0.1

### Added

- Root sitemap validation to prevent nested sitemap indexes
- Automatic detection and logging of nested sitemap indexes
- Dashboard links for Main Sitemap and Google News Sitemap
- Improved Cloudflare cache rule recommendations

### Improved

- Root sitemap now publishes only final sitemap files
- Improved Google Search Console compatibility
- Updated robots.txt sitemap integration
- Improved XML validation during sitemap publication
- Enhanced production stability

### Unchanged

- Scheduler architecture
- Archive engine
- Content providers
- Sitemap generation workflow

---

## Author

**Kostas Stathopoulos**  
DevArt

https://devart.gr

GitHub Repository:

https://github.com/devartgr/joomla-devart-sitemaps

---

## License

GNU General Public License v3.0 (GPLv3)

---

## Disclaimer / Limitation of Liability

This software is provided "as is", without warranty of any kind.

DevArt shall not be held liable for any damages, data loss, downtime, security incidents, business interruption, loss of profits, or other consequences arising from the use or inability to use this software.

Always test updates in a staging environment before deploying to production systems.
