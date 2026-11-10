# Hi, I'm Shon Bida

Security researcher hunting vulnerabilities in WordPress plugins and open-source web apps (PHP, Laravel, Django). Coordinated disclosure through Wordfence, Patchstack, VulnCheck, GitHub Security Advisories and HackerOne.

![Published CVEs](https://img.shields.io/badge/Published%20CVEs-5-c0392b?style=flat-square) ![Advisories](https://img.shields.io/badge/Advisories-6-8e44ad?style=flat-square) ![In disclosure](https://img.shields.io/badge/In%20disclosure-16-7f8c8d?style=flat-square) [![HackerOne](https://img.shields.io/badge/HackerOne-Milestone%20Level%201-494649?style=flat-square)](https://hackerone.com/dexx-tech) [![HackerOne](https://img.shields.io/badge/HackerOne-Milestone%20Level%202-494649?style=flat-square)](https://hackerone.com/dexx-tech) [![HackerOne](https://img.shields.io/badge/HackerOne-Milestone%20Level%203-494649?style=flat-square)](https://hackerone.com/dexx-tech)

**Find me on:** [HackerOne](https://hackerone.com/dexx-tech) · [Patchstack](https://patchstack.com/database/researchers/624003fb-5f41-43f3-b5fa-c26032e482e4) · [LinkedIn](https://www.linkedin.com/in/shon-bida)

## Published vulnerabilities

| ID | Product | Vulnerability | Access | CVSS 3.1 | Affected | Fixed in |
|---|---|---|---|---|---|---|
| [CVE-2026-122666](https://patchstack.com/database/wordpress/plugin/mangboard/vulnerability/wordpress-mang-board-wp-plugin-2-4-7-cross-site-scripting-xss-vulnerability) | Mang Board WP (WordPress) | **Cross-Site Scripting** (CWE-79): editing an owned post flips it to HTML mode, so the unpurified stored body renders as script on the public view page. | Subscriber | 7.1 High | <= 2.4.7 | 2.4.8 |
| [CVE-2026-39738](https://patchstack.com/database/wordpress/plugin/wp-marketing-automations/vulnerability/wordpress-funnelkit-automations-plugin-3-8-6-1-php-object-injection-vulnerability) | FunnelKit Automations (WordPress) | **PHP Object Injection** (CWE-502): checkout address text from a shopper is stored raw and later PHP-unserialized, giving an unauthenticated object injection primitive. | Unauthenticated | 9.8 Critical | <= 3.8.6.1 | 3.8.6.2 |
| [GHSA-jrgm-fhgv-hmj9](https://github.com/wagtail/wagtail/security/advisories/GHSA-jrgm-fhgv-hmj9) | Wagtail | **Improper Authorization** (CWE-285): the v3 pages API returns unpublished drafts and pages outside the user's permissions to any token-authenticated user. | Authenticated (API token) | 4.3 Medium | 8.0 | 8.0.1 |
| [CVE-2026-116746](https://www.cve.org/CVERecord?id=CVE-2026-116746) | QloApps | **Missing Authorization** (CWE-862): anyone can post forged hotel reviews and ratings for arbitrary orders. | Unauthenticated | 5.3 Medium | 1.6.0 - 1.7.0 | develop ([#1757](https://github.com/Qloapps/QloApps/pull/1757)), unreleased |
| [CVE-2026-116745](https://www.cve.org/CVERecord?id=CVE-2026-116745) | QloApps | **IDOR** (CWE-639): enumerating guest cart IDs leaks the customer's email, order reference and secure key, leading to invoice disclosure and account takeover. | Unauthenticated | 6.5 Medium | <= 1.7.0 | develop ([#1912](https://github.com/Qloapps/QloApps/pull/1912)), unreleased |
| [CVE-2026-107706](https://www.cve.org/CVERecord?id=CVE-2026-107706) | Dolibarr ERP CRM | **Missing Authorization** (CWE-862): a read-only user can change extra-field values on records through the extra-field AJAX endpoint. | Low-privilege user | 4.3 Medium | < 24.0.2 | 24.0.2 |

Plus **16 more** reports in coordinated disclosure (GitHub, HackerOne, Patchstack, Vendor, VulnCheck, Wordfence). They will be listed here once the vendors have fixed them and the advisories are public.
