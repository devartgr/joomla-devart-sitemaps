# DevArt Sitemaps for Joomla

Professional Joomla 6 XML sitemap solution designed for business websites, news portals, magazines, municipalities, organizations, enterprise deployments, and high-performance websites with small or very large content collections.

![Joomla](https://img.shields.io/badge/Joomla-6.x-blue)
![PHP](https://img.shields.io/badge/PHP-8.2%2B-green)
![Release](https://img.shields.io/badge/Version-1.0.0-orange)
![License](https://img.shields.io/badge/License-GPLv3-red)

---

## Overview

DevArt Sitemaps is a modern Joomla 6 native XML sitemap generator built for performance, scalability, reliability and production deployments.

Instead of generating XML dynamically on every request, DevArt Sitemaps builds static XML files that can be served efficiently by Joomla, web servers and CDNs, dramatically reducing database load while providing excellent scalability for high-traffic websites.

The extension supports multiple content providers, automatic archive generation, Google News sitemaps, Joomla Scheduled Tasks and enterprise-scale sitemap management.

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

- Automatic sitemap generation
- Provider-based architecture
- Provider-specific indexes
- Sitemap splitting
- XML validation
- Automatic rebuild tools

---

### Google News

Built-in Google News sitemap generation.

Features include:

- Recent news support
- Automatic updates
- XML validation
- Google News compatible format

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

- Sitemap statistics
- Scheduler status
- Build history
- Activity logs
- Provider overview
- System health information

---

### Performance

Built for production environments.

Features:

- Static XML generation
- Optimized database queries
- Minimal server load
- Cloudflare friendly
- CDN friendly
- Large dataset support
- Low memory usage

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
- Server-side validation
- Secure file operations

Designed for secure production deployments.

---

## Compatibility

Supported:

- Joomla 6.x
- PHP 8.2+
- Joomla native updates
- Joomla Scheduled Tasks
- Modern Joomla MVC architecture

Not Supported:

- Joomla 3
- Joomla 4
- Joomla 5
- Legacy PHP versions

---

## Current Version

**1.0.0**

---

## What's New in 1.0.0

### Added

- Static XML sitemap engine
- Joomla Articles support
- DevArt Business support
- DevArt Events support
- DevArt Video support
- Google News sitemap generation
- Provider-based architecture
- Monthly archive generation
- Joomla Scheduled Tasks integration
- Build history and activity logs
- Dashboard with scheduler monitoring
- Joomla Update Server support

### Improved

- Joomla 6 native architecture
- Optimized XML generation
- Reduced database load
- Cloudflare compatibility
- Enterprise-ready scalability
- Production-safe build process

### Compatibility

- Joomla 6 native architecture
- PHP 8.2+
- Production-ready release

---

## Author

Kostas Stathopoulos  
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
