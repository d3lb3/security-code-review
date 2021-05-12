# Security Code Review Resources

My personal collection of resources (mostly tools and training materials) for source code security audits. Updated gradually as I discover interesting material on the subject.

* [**Training Materials**](#training-materials)
  * [Learning Resources](#learning-resources)
  * [Learning Platforms](#learning-platforms)
  * [Vulnerable Apps](#vulnerable-apps)
* [**Tools**](#tools)
  * [Static Application Security Testing (SAST) Tools](#static-application-security-testing-sast-tools)
  * [Grep-based Tools](#grep-based-tools)
  * [Frameworks](#frameworks)
* [**Lists**](#lists)
  * [Vulnerability Checklists](#vulnerability-checklists)
  * [Interesting Keywords &amp; Regex](#interesting-keywords--regex)
 
## Training Materials

### Learning Resources

- [[Blog Post] Secure Code Review (MITRE's System Engineering Guide)](https://www.mitre.org/publications/systems-engineering-guide/enterprise-engineering/systems-engineering-for-mission-assurance/secure-code-review) : good introduction with definitions.
- [[Conference] OWASP Appsec Day - The Absolute AppSec Secure Code Review Framework](https://www.youtube.com/watch?v=Kepd1HsoE8o) : strong focus on methodology.
- [[Conference] Source code security audit speed run by Eldar Marcussen](https://www.youtube.com/watch?v=hpYjjj1UAXs) : methodology and tooling.
- [[Guide] OWASP Code Review Guide (currently v2)](https://owasp.org/www-pdf-archive/OWASP_Code_Review_Guide_v2.pdf) : (almost) exhaustive guide on secure code review.

### Learning Platforms

- [OWASP's Secure Coding Dojo Example](https://owasp.org/SecureCodingDojo/codereview101)
- [Secure Code Warrior](https://www.securecodewarrior.com/products/training-ground) (paid service with free trial)

### Vulnerable Apps

- [Vulnerable Task Manager (vtm)](https://github.com/redpointsec/vtm) : vulnerable task manager in Python/Django, correction not available.
- [OWASP WebGoat](https://github.com/WebGoat/WebGoat) : vulnerable web application with Java backend, correction available.
- [Damn Vulnerable iOS App 1](https://github.com/prateek147/DVIA) : vulnerable iOS app written in Objective-C, correction available.
- [Damn Vulnerable iOS App 2](https://github.com/prateek147/DVIA-v2) : vulnerable iOS app written in Swift, correction available.

## Tools

### Static Application Security Testing (SAST) Tools

- [OWASP's Source Code Analysis Tools](https://owasp.org/www-community/Source_Code_Analysis_Tools)
- [A curated list of static analysis tools and tools and config files (GitHub)](https://github.com/analysis-tools-dev/static-analysis)
- [Static Application Security Testing Suites used in GitLab's CI/CD](https://docs.gitlab.com/ee/user/application_security/sast/)

### Grep-based Tools

- [megagrep](https://github.com/claire-lex/megagrep) : find interesting parts of the code to manually check based on keywords. Comes with additional features such as per-file statistics or dev comments search.
- [graudit](https://github.com/wireghoul/graudit) : find very specific vulnerabilities based on regular expressions, a lot of false negatives but can be extended with your own regexs.
- [crass](https://github.com/floyd-fuh/crass) : source code grep-er with a set of selected high-potential strings that may result in (security) problems.
- [drek](https://github.com/chrisallenlane/drek) : source code grep-er with nice HTML and PDF reports.
- [DumpsterDiver](https://github.com/securing/DumpsterDiver) : search secrets based on entropy.
- [Code-Crawler](https://github.com/vmnguyen/Code-Crawler) : automatic tool used for crawling code to find low-hanging fruits.

### Frameworks

- [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF) : all-in-one mobile application (Android/iOS/Windows) pen-testing, malware  analysis and security assessment framework capable of performing static  and dynamic analysis.

## Lists

### Vulnerability Checklists

- [Michaela Greiler's checklist](https://github.com/mgreiler/secure-code-review-checklist)
- [Aggregated checklist from various sources](https://github.com/softwaresecured/secure-code-review-checklist)
- [OWASP's Code Review Checklist](https://owasp.org/www-pdf-archive/OWASP_Code_Review_Guide_v2.pdf#page=197)
- [My own custom list based on the above resources](https://github.com/JulienBedel/security-code-review/blob/main/Security_Code_Review_Helper.xlsx)

### Interesting Keywords & Regex

- [OWASP's Code Review Keywords List](https://owasp.org/www-pdf-archive/OWASP_Code_Review_Guide_v2.pdf#page=207)
- [Collection of Regex in various languages](https://github.com/va1da5/manual-source-code-review)
- [My own Keywords List](https://github.com/JulienBedel/security-code-review/tree/main/keywords)

